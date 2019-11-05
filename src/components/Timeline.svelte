<script>
	export const entries = [
    {
      type: 'fuel',
      price: 100,
      date: new Date(2019, 8, 23),
      speedometer: 1300
    },
    {
      type: 'treatment',
      price: 200,
      date: new Date(2019, 9, 23),
      speedometer: 1500
    },
  ];
</script>

<div class="ui feed">
  {#each entries as item}
    <div class="event">
      <div class="label">
        <img alt="" src="/assets/icons/fuel.svg">
      </div>
      <div class="content">
        <div class="summary">
          {item.type}
          <div class="date">
            {item.date.toLocaleString()}
          </div>
        </div>
        <div class="meta">
          {item.speedometer}km
        </div>
      </div>
    </div>
  {/each}
  <div class="event">
    <div class="label">
      <img alt="" src="/assets/icons/fuel.svg">
    </div>
    <div class="content">
      <div class="summary">
        <a class="user">
          Elliot Fu
        </a> added you as a friend
        <div class="date">
          1 Hour Ago
        </div>
      </div>
      <div class="meta">
        <a class="like">
          <i class="like icon"></i> 4 Likes
        </a>
      </div>
    </div>
  </div>
  <div class="event">
    <div class="label">
      <img alt="" src="/assets/icons/fuel.svg">
    </div>
    <div class="content">
      <div class="summary">
        <a>Helen Troy</a> added <a>2 new illustrations</a>
        <div class="date">
          4 days ago
        </div>
      </div>
      <div class="extra images">
        <a><img src="/images/wireframe/image.png"></a>
        <a><img src="/images/wireframe/image.png"></a>
      </div>
      <div class="meta">
        <a class="like">
          <i class="like icon"></i> 1 Like
        </a>
      </div>
    </div>
  </div>
  <div class="event">
    <div class="label">
      <img alt="" src="/assets/icons/fuel.svg">
    </div>
    <div class="content">
      <div class="summary">
        <a class="user">
          Jenny Hess
        </a> added you as a friend
        <div class="date">
          2 Days Ago
        </div>
      </div>
      <div class="meta">
        <a class="like">
          <i class="like icon"></i> 8 Likes
        </a>
      </div>
    </div>
  </div>
  <div class="event">
    <div class="label">
      <img alt="" src="/assets/icons/fuel.svg">
    </div>
    <div class="content">
      <div class="summary">
        <a>Joe Henderson</a> posted on his page
        <div class="date">
          3 days ago
        </div>
      </div>
      <div class="extra text">
        Ours is a life of constant reruns. We're always circling back to where we'd we started, then starting all over again. Even if we don't run extra laps that day, we surely will come back for more of the same another day soon.
      </div>
      <div class="meta">
        <a class="like">
          <i class="like icon"></i> 5 Likes
        </a>
      </div>
    </div>
  </div>
  <div class="event">
    <div class="label">
      <img alt="" src="/assets/icons/fuel.svg">
    </div>
    <div class="content">
      <div class="summary">
        <a>Justen Kitsune</a> added <a>2 new photos</a> of you
        <div class="date">
          4 days ago
        </div>
      </div>
      <div class="extra images">
        <a><img src="/images/wireframe/image.png"></a>
        <a><img src="/images/wireframe/image.png"></a>
      </div>
      <div class="meta">
        <a class="like">
          <i class="like icon"></i> 41 Likes
        </a>
      </div>
    </div>
  </div>
</div>