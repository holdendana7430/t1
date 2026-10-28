代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://hz.smart0.xyz/gtxkungnin.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.redwolf501.top/gtbhbzpeif.html

[Q13] 忽略重复插入
来源：http://hz.0kj1m.cn/gtqosxtnux.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.zhengqikj.top/gtbjjrbjsz.html

[Q14] 存在则更新（upsert）
来源：http://hz.hywenlv.cn/gtosgiwviv.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.pycfn.com/gtttdrlkzu.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.xuanzx.com/gtbfmrxxtd.html

[Q15] 查询全部
来源：http://hz.jinqigfzy.top/gtmdbdlmhw.html

SELECT * FROM users;
来源：http://hz.tianlin.xyz/gtdxfjypkr.html

[Q16] 查询指定列
来源：http://hz.aizwys.cn/gtxvbcwopp.html

SELECT id, name FROM users;
来源：http://hz.jinyuanbaomall.cn/gtqzxforvn.html

[Q17] 条件查询
来源：http://hz.daria6918.cn/gtyiazqqmc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigufen.top/gtnnwzvjzo.html

[Q18] 模糊匹配
来源：http://hz.zhoulong.xyz/gtbqodhekf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.nwbrower.top/gthyfuptll.html

[Q19] 范围查询
来源：http://hz.smart0.xyz/gtcxxuqdwv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yuanzhike.top/gtmykwaqpw.html

[Q20] IN 列表
来源：http://hz.jyoumei.cn/gtqxyviigc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.tanke756.top/gtkbphlaps.html

[Q21] 空值判断
来源：http://hz.yongpay.top/gtxpfigltv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.vqdsnc.cn/gtkpjrqyyz.html

[Q22] 排序
来源：http://hz.meibo888.top/gtgljxeklq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.ybcxt.top/gtegsfrenn.html

[Q23] 分页
来源：http://hz.chenlongwang.top/gtodzxvqjl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.zhaomingkeji.xyz/gtumpglfjr.html

[Q24] 去重
来源：http://hz.iojbl.cn/gtdfohtcyh.html

SELECT DISTINCT city FROM users;
来源：http://hz.ydzc1.top/gttmhbmefl.html

[Q25] 只取前 N 条
来源：http://hz.daria6918.cn/gtwwjhcnfa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.snrcjt.cn/gtmwgyqhwq.html

[Q26] 计数
来源：http://hz.vqdsnc.cn/gtoxsgforb.html

SELECT COUNT(*) FROM users;
来源：http://hz.kuanghao11.cn/gtpjesojms.html

[Q27] 条件计数
来源：http://hz.daria6918.cn/gtvasiypmp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jqgufenzy.top/gtdhlgybgu.html

[Q28] 求和与平均
来源：http://hz.zhaomingkeji.xyz/gtimrwnnmr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.xylfe.cn/gtmbmndnxq.html

[Q29] 最大最小值
来源：http://hz.jinyuanbaomall.cn/gtmbwtbnye.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.haohaochexian.top/gtwasnhnrc.html

[Q30] 分组统计
来源：http://hz.0kj1m.cn/gtdtmcmklb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xinyue.icu/gtggllhytd.html

[Q31] 分组后过滤
来源：http://hz.guannengcc.top/gtfjkczpmx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hnxiangtu.top/gtimugvfxa.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gtlfprqxag.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtiudmeflx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.iojbl.cn/gtqqclbfts.html

[Q33] 多列分组
来源：http://hz.xylfe.cn/gtolgqlbes.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ybcxt.top/gtxbfdfgyr.html

[Q34] 每组取第一条
来源：http://hz.xuetiantiany.cn/gtybgbeuzg.html

SELECT * FROM (
来源：http://hz.birdmap.top/gtdeubaqgo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.daxiang520.top/gtekzcbpjg.html

) t WHERE rn = 1;
来源：http://hz.dianchejie.cn/gtboewdava.html

[Q35] 内连接
来源：http://hz.hnqzz.top/gtmafqbdvz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtyqzevrxm.html

[Q36] 左连接
来源：http://hz.dianchejie.cn/gtwfikcmtb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cucudq.cn/gtecsirfag.html

[Q37] 右连接
来源：http://hz.xinyue.icu/gtwasplmgy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.cheryme.top/gthffwpexe.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sweek.top/gthhzfeogb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnqzz.top/gthykyucqk.html

[Q39] 自连接（查上下级）
来源：http://hz.xylfe.cn/gtgwdittvj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yj20258.top/gtyxdpggjx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ybcxt.top/gtuvqphube.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinghuilouyu.cn/gtdfyahkvv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtfrjxczai.html

[Q41] 多表连接
来源：http://hz.haohaochexian.top/gtcdrvbbii.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinyuanbaomall.cn/gtqbkeosel.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cashguo.top/gtndcnpwtx.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhiwuduotai.top/gtyjbfxqkj.html

[Q42] 连接条件附加过滤
来源：http://hz.zhixingplan.top/gtmezuemav.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shzxlz.cn/gtbmqxbiir.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.daxiang520.top/gtrkbgbjsm.html

[Q43] 标量子查询
来源：http://hz.feifeiyinyue.top/gtmgtypkvh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ehwqpu.com/gtkceotmap.html

[Q44] IN 子查询
来源：http://hz.hongshengwenyu.top/gtbotdjnwq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yj20258888.top/gtxqxygewy.html

[Q45] EXISTS 判断存在
来源：http://hz.haohaochexian.top/gtllydcovv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenlongwang.top/gtizjgsoaz.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yvedp.cn/gttysmvkwv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shanyushiyangtech.top/gtqebcrsep.html

[Q47] 与平均值比较
来源：http://hz.haohaochexian.top/gtxznajxdb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gtlxcbqrhp.html

[Q48] CTE 公用表表达式
来源：http://hz.tian-w.cn/gteiryemfc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.sysykeji.top/gthtldwakq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.meibo888.top/gtecfydzgz.html

[Q49] 更新单行
来源：http://hz.quarkkingdee.top/gtshrbjhni.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.pengpengdd.cyou/gtjfyuhdke.html

[Q50] 批量更新
来源：http://hz.wangdashe.top/gtkdhhzkzm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zhijiandao.cn/gtwrinugin.html

[Q51] 用子查询更新
来源：http://hz.tianlin.xyz/gtdzwjkwxp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.shuidangran.top/gtqdkobgev.html

[Q52] 删除指定行
来源：http://hz.quarkkingdee.top/gtikbklxsm.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gtyusaxomx.html

[Q53] 按条件删除
来源：http://hz.yangfankeji.com/gtagoyqyvu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gaohongyu789.top/gtrrgkkpmv.html

[Q54] 清空表
来源：http://hz.fzhhl.top/gtlcngjmna.html

TRUNCATE TABLE logs;
来源：http://hz.fzhhl.top/gtwccouabh.html

[Q55] 排名（并列占位）
来源：http://hz.guannengcc.top/gtbqrifbwm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jyoumei.cn/gtztupxmlz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nwbrower.top/gtvlozdjok.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxinkj.top/gttefarxlx.html

[Q57] 行号
来源：http://hz.chenjidiqi.icu/gttffyppkj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinyuanbaomall.cn/gtaeqebndl.html

[Q58] 累计求和
来源：http://hz.ydjk.org.cn/gtgydoqgpd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgufenzy.top/gttathdymw.html

[Q59] 分组内累计
来源：http://hz.xingfuxueyuan.xyz/gtgxdqrioa.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.chenzaomai.com/gtwsdhhuuu.html

[Q60] 取上一行 / 下一行
来源：http://hz.ybcxt.top/gtviymiyva.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yongpay.top/gtihzusogj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.pycfn.com/gtiwtlinbw.html

[Q61] 移动平均
来源：http://hz.aibaodan.cn/gtmgrnxzsl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.wangshuangyany.cn/gtlbepfcho.html

[Q62] 分组占比
来源：http://hz.dianchejie.cn/gtdztvigmc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yongpay.top/gtmidxtsml.html

[Q63] 开启事务
来源：http://hz.pengpengdd.cyou/gtbpzkkpgb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sxryk.cn/gtrzmaxzqh.html

[Q64] 提交事务
来源：http://hz.xingfuxueyuan.xyz/gtapoicgtu.html

COMMIT;
来源：http://hz.vqdsnc.cn/gtxwitzuvz.html

[Q65] 回滚事务
来源：http://hz.shanyushiyangtech.top/gtdbuhogsk.html

ROLLBACK;
来源：http://hz.yvedp.cn/gtdmlqijwg.html

[Q66] 行锁查询
来源：http://hz.yangfankeji.com/gtopllgwvh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gotoacloud.top/gtjinfyuww.html

[Q67] 设置隔离级别
来源：http://hz.jlsjyb.cn/gtedgtsyff.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pycfn.com/gthebezhqu.html

[Q68] 保存点
来源：http://hz.cdnleiting.top/gtyjrxzjbv.html

SAVEPOINT sp1;
来源：http://hz.aibaodan.cn/gtqkfgeifg.html

ROLLBACK TO sp1;
来源：http://hz.aizwys.cn/gtibudxgvg.html

[Q69] 查看执行计划
来源：http://hz.guowangkeji.top/gtgqfsdqjj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.daria6918.cn/gtfrxkmugy.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangtech.top/gtfvhrqhyh.html

ANALYZE TABLE users;
来源：http://hz.aibaodan.cn/gtgilhkmcs.html

[Q71] 查看建表语句
来源：http://hz.nanxuanxn.top/gtwsfceacr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zdqjudy.top/gtgpyvxioi.html

[Q72] 查看索引
来源：http://hz.jqgufenzy.top/gtljkcdwaf.html

SHOW INDEX FROM users;
来源：http://hz.jiagoushi.top/gtvxusnbfi.html

[Q73] 查看表状态
来源：http://hz.zhaomingkeji.xyz/gtzgdxphiv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.chenlongwang.top/gtwkyzciqx.html

[Q74] 强制使用索引
来源：http://hz.hysaishi.cn/gtsodbfdgy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yueranfly.top/gthridtwvp.html

[Q75] 日期格式化
来源：http://hz.shuidangran.top/gthhzjhyup.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuxming.cn/gtbzmaiayj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.shanyushiyangkeji.top/gtqpavebyg.html

[Q76] 按天统计
来源：http://hz.ydjk.org.cn/gtslhayfah.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cheryme.top/gtovrktrrr.html

[Q77] 时间加减
来源：http://hz.feifeiyinyue.top/gtaafsrjcj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hywenlv.cn/gtdrljdvos.html

[Q78] 当前时间
来源：http://hz.bjfxy.top/gthhvxgkpr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jianghu66.top/gtwzdrugyf.html

[Q79] 字符串拼接
来源：http://hz.aizwys.cn/gtuklgaoci.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yonumen.top/gtpvfrldij.html

[Q80] 字符串截取
来源：http://hz.meibo888.top/gtgyyimtac.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yueranfly.top/gtrbvyjjed.html

[Q81] 字符串替换
来源：http://hz.yvedp.cn/gtghvgnzub.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xylfe.cn/gtnccepocs.html

[Q82] 字符长度与字节长度
来源：http://hz.9152youxi.cn/gtzplagbtx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yangfankeji.com/gttsuqmuam.html

[Q83] 大小写转换
来源：http://hz.jinqigfzy.top/gtacfmiero.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xylfe.cn/gtmoticdyb.html

[Q84] 去除首尾空格
来源：http://hz.shuidangran.top/gtmlzgxcsi.html

SELECT TRIM(name) FROM users;
来源：http://hz.cdnleiting.top/gtetnaanwe.html

[Q85] 数值取整
来源：http://hz.redwolf501.top/gtkbppbkol.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cucudq.cn/gtbshhwopj.html

[Q86] 读取 JSON 字段
来源：http://hz.cheryme.top/gtefjpzckj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yvedp.cn/gtkklqshfd.html

[Q87] JSON 字段做条件
来源：http://hz.yueranfly.top/gtriyrafnr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hysaishi.cn/gtmichgnlm.html

[Q88] 行转列（条件聚合）
来源：http://hz.hammf.cn/gtrpazmsdj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.316326.xyz/gtjfodfgxe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ehwqpu.com/gtucrbkpjy.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gteapxvqpn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ybcxt.top/gtjhppugye.html

[Q90] 生成序号列
来源：http://hz.jyoumei.cn/gtzyhllnnr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnxiangtu.top/gtzdfqigmx.html

================================================================================
来源：http://hz.birdmap.top/gtqxclisfi.html

R. Bash 专题
来源：http://hz.andypj.xyz/gtxhlowhjo.html

================================================================================
来源：http://hz.sufxvd.cn/gtjdlfgksr.html

[R01] shebang 与严格模式
来源：http://hz.gogol.net.cn/gtlfspnvjr.html

#!/usr/bin/env bash
来源：http://hz.aibaodan.cn/gtsqkncuxd.html

set -euo pipefail
来源：http://hz.ydzc1.top/gtijtxfgrd.html

[R02] 变量赋值与使用
来源：http://hz.feifeiyinyue.top/gtnxbzvdlx.html

name="Tom"; echo "$name"
来源：http://hz.nanxinkj.top/gtlcmndjmj.html

[R03] 只读变量
来源：http://hz.vqdsnc.cn/gtamqsfjza.html

readonly PI=3.14
来源：http://hz.meibo888.top/gtgkdhgyyp.html

[R04] 位置参数
来源：http://hz.0kj1m.cn/gtndilumba.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangdashe.top/gtkfnwspgt.html

[R05] 参数默认值
来源：http://hz.tianlin.xyz/gtnocbptat.html

name="${1:-default}"
来源：http://hz.gotoacloud.top/gtsurmqspu.html

[R06] 判断命令是否存在
来源：http://hz.jqgufenzy.top/gtacwhnjpe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtfemdozrp.html

[R07] if 判断文件
来源：http://hz.yuanzhike.top/gtovrsonnp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cdnleiting.top/gthcuaqgph.html

[R08] 数值比较
来源：http://hz.hfpthk.cn/gtpnmnmrrz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.haohaochexian.top/gtwpbhvtdn.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtnatmpmds.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sweek.top/gtosbkvzev.html

[R10] 正则匹配
来源：http://hz.hnxiangtu.top/gtheeffthx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ppjwa.cn/gtegndhgqm.html

[R11] case 多分支
来源：http://hz.zdqjudy.top/gtqysgtmqz.html

case "$1" in
来源：http://hz.shanyushiyangtech.top/gtdntcgisx.html

start) echo "启动" ;;
来源：http://hz.zhongyouzk.top/gturwwbqnb.html

stop)  echo "停止" ;;
来源：http://hz.wangshuangyany.cn/gtvzzpcxdr.html

*)     echo "未知命令" ;;
来源：http://hz.birdmap.top/gtaueykdlj.html

esac
来源：http://hz.ywan-chungtsiang.top/gtkwaqpgyk.html

[R12] for 遍历文件
来源：http://hz.jiagoushi.top/gtaikvmebe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.feifeiyinyue.top/gthhjlyvzc.html

[R13] for 计数循环
来源：http://hz.316326.xyz/gtizftkxmh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.meibo888.top/gtzavcucxx.html

[R14] C 风格 for
来源：http://hz.yongpay.top/gtamhzzomk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gzhubu.top/gtkglamlvb.html

[R15] while 逐行读文件
来源：http://hz.ybcxt.top/gtpxpsvcob.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigfzy.top/gtvszevhae.html

[R16] until 等待条件
来源：http://hz.vqdsnc.cn/gthstljcam.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenlongwang.top/gtzmrbxhyt.html

[R17] 数组定义与取值
来源：http://hz.sufxvd.cn/gtaqgyrdkg.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgfzy.top/gtztwscmaw.html

[R18] 遍历数组
来源：http://hz.svipenyu.cn/gtcldtxkhm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jyoumei.cn/gtnhtnwxls.html

[R19] 数组长度
来源：http://hz.jinqigufen.top/gtvxdezyya.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gthxdtfpoq.html

[R20] 关联数组（字典）
来源：http://hz.xziqi.cn/gtyufbloho.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj202588.top/gtkcdunbgv.html

[R21] 字符串长度
来源：http://hz.guowangkeji.top/gtygmilllt.html

echo "${#s}"
来源：http://hz.sxryk.cn/gtqdwatnas.html

[R22] 截取子串
来源：http://hz.pycfn.com/gthzgkgpfy.html

echo "${s:0:5}"
来源：http://hz.hywenlv.cn/gtdjpylfrl.html

[R23] 字符串替换
来源：http://hz.zhengqikj.top/gtcjhimjpj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yangfankeji.com/gtqpydmskp.html

[R24] 大小写转换
来源：http://hz.nanxinkj.top/gtcwlehcma.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.c1oappe.top/gtkiksceef.html

[R25] 去后缀 / 去前缀
来源：http://hz.yongpay.top/gtmtgadzcn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuxming.cn/gtwkgontvy.html

[R26] 命令替换
来源：http://hz.jlsjyb.cn/gtoajlairl.html

now=$(date +%F); echo "$now"
来源：http://hz.yvedp.cn/gtmkyqagvu.html

[R27] 算术展开
来源：http://hz.zhijiandao.cn/gtmkfzyrks.html

echo $((1 + 2 * 3))
来源：http://hz.tianlin.xyz/gtdnxlelmo.html

[R28] 浮点运算
来源：http://hz.cdnleiting.top/gthvgedmbr.html

echo "scale=2; 10/3" | bc
来源：http://hz.pycfn.com/gtuluyfpso.html

[R29] 定义函数
来源：http://hz.feifeiyinyue.top/gtobtbgcwb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cqqwz.cn/gtaajoryqt.html

[R30] 函数返回状态码
来源：http://hz.guannengcc.top/gtgefhxgwi.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gtwkagqsuw.html

[R31] 局部变量
来源：http://hz.tian-w.cn/gtvmibcmep.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxinkj.top/gtxfhokxmw.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gtgghunkzq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuanzhike.top/gtzsvujhwd.html

[R33] 捕获错误并提示行号
来源：http://hz.wangdashe.top/gtfsdwbrvz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.meibo888.top/gtyyflirlq.html

[R34] 退出时清理
来源：http://hz.c1oappe.top/gtyooswtub.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jyoumei.cn/gtwlgsrwsb.html

[R35] 后台执行并等待
来源：http://hz.hysaishi.cn/gtuzspnhqf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yangfankeji.com/gtxtkrfazx.html

[R36] 并发执行多个任务
来源：http://hz.gotoacloud.top/gtnacgihvs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hammf.cn/gtkbqjgukt.html

[R37] 把输出赋给变量
来源：http://hz.fengsongda.top/gtdkqtxsmx.html

files=$(ls -1)
来源：http://hz.gotoacloud.top/gttkvespqs.html

[R38] 管道串联
来源：http://hz.jianghu66.top/gtcwuhjxfx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtrdwtagbf.html

[R39] 重定向标准输出与错误
来源：http://hz.pycfn.com/gtoydhswnj.html

cmd > out.log 2>&1
来源：http://hz.xylfe.cn/gtdygrzuwd.html

[R40] 追加写日志
来源：http://hz.ywan-chungtsiang.top/gtqddzwrbu.html

echo "log" >> out.log
来源：http://hz.svipenyu.cn/gtdndiojrt.html

[R41] 丢弃输出
来源：http://hz.cdnleiting.top/gtbysnxjsv.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gtoofbpqdv.html

[R42] 输入重定向
来源：http://hz.shzxlz.cn/gtnfxrqxls.html

wc -l < a.txt
来源：http://hz.daria6918.cn/gtpcvngyht.html

[R43] 按名字查找文件
来源：http://hz.vqdsnc.cn/gtmnsafkbr.html

find . -name "*.log" -type f
来源：http://hz.snrcjt.cn/gtaidixddi.html

[R44] 按修改时间查找
来源：http://hz.nanxuanxn.top/gtgeydyvma.html

find . -mtime -7 -type f
来源：http://hz.havefunace.top/gtmxgwagun.html

[R45] 批量删除
来源：http://hz.gaohongyu789.top/gtzpvwbfzv.html

find . -name "*.tmp" -delete
来源：http://hz.nanxinkj.top/gtddemhcul.html

[R46] 递归替换文件内容
来源：http://hz.sysykeji.top/gtmppxebzc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hongshengwenyu.top/gtnbdkgxxg.html

[R47] sed 单行替换
来源：http://hz.hfpthk.cn/gtpypuwsyb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xziqi.cn/gtuceqkjny.html

[R48] awk 取指定列
来源：http://hz.ydzc1.top/gtnywxkrqf.html

awk '{print $1, $3}' a.txt
来源：http://hz.9152youxi.cn/gtbtdyxulx.html

[R49] awk 带条件
来源：http://hz.dianchejie.cn/gtrzotcjmf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.meibo888.top/gtztxhrlqp.html

[R50] awk 求和
来源：http://hz.xuetiantiany.cn/gthdgehyiy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.andypj.xyz/gtaczswbbs.html

[R51] 排序去重取前几
来源：http://hz.zhiwuduotai.top/gtemnaflyv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guowangkeji.top/gtbhiklobo.html

[R52] 统计行数
来源：http://hz.gotoacloud.top/gtvinticjv.html

wc -l a.txt
来源：http://hz.hongshengwenyu.top/gtfyyvhipn.html

[R53] 查看文件头与实时尾
来源：http://hz.guannengcc.top/gtirsnxzeu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ppjwa.cn/gtsnkkbomp.html

[R54] 比较两个文件
来源：http://hz.ivvv.top/gtmxriypiy.html

diff a.txt b.txt
来源：http://hz.tanke756.top/gtynrggqab.html

[R55] 压缩与解压
来源：http://hz.havefunace.top/gtrbsqvyhl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xylfe.cn/gtoqtviwxl.html

[R56] 远程拷贝
来源：http://hz.jianghu66.top/gtcuphjqos.html

scp file user@host:/path/
来源：http://hz.birdmap.top/gtplquecch.html

[R57] 远程执行命令
来源：http://hz.shangyingyoupin.top/gtosusbyta.html

ssh user@host 'uptime'
来源：http://hz.dashuyun.cn/gtmiztpgix.html

[R58] 下载文件
来源：http://hz.zhoulong.xyz/gtjtsptedx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinghuilouyu.cn/gttepidjvo.html

[R59] 发 POST JSON
来源：http://hz.cucudq.cn/gteyfktigu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.redwolf501.top/gtvflkibet.html

[R60] 只看 HTTP 状态码
来源：http://hz.ydjk.org.cn/gtqcambddp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhoulong.xyz/gtpalasbok.html

[R61] 磁盘占用
来源：http://hz.xylfe.cn/gtpmsxsonj.html


<!-- 参考信息 -->