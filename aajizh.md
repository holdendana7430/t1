代发 wailian999

SELECT * FROM users;
来源：http://hz.yueranfly.top/gtcvevplxd.html

[Q16] 查询指定列
来源：http://hz.hywenlv.cn/gtfqhnvubg.html

SELECT id, name FROM users;
来源：http://hz.yangfankeji.com/gtauoqaczo.html

[Q17] 条件查询
来源：http://hz.jiagoushi.top/gtcafiskmz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.9152youxi.cn/gtxqfpvyln.html

[Q18] 模糊匹配
来源：http://hz.daxiang520.top/gtnidqbqnx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shanyushiyangkeji.top/gtwuxtgoay.html

[Q19] 范围查询
来源：http://hz.gogol.net.cn/gtchbqddju.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zhengqikj.top/gtqvytnfha.html

[Q20] IN 列表
来源：http://hz.pycfn.com/gtthhyrzkw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.dashuyun.cn/gtkbyhgvps.html

[Q21] 空值判断
来源：http://hz.jinqigfzy.top/gtjxmknkqp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.guannengcc.top/gtanvtfhbo.html

[Q22] 排序
来源：http://hz.andypj.xyz/gtjovmogre.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.zdqjudy.top/gtjmntcewj.html

[Q23] 分页
来源：http://hz.hfpthk.cn/gtnyzrghtp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.yangfankeji.com/gtswomedkg.html

[Q24] 去重
来源：http://hz.nanxuanxn.top/gtquyyelsc.html

SELECT DISTINCT city FROM users;
来源：http://hz.gzhubu.top/gthutfrroc.html

[Q25] 只取前 N 条
来源：http://hz.cashguo.top/gttnqmfahj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.ydzc1.top/gtbasloiqp.html

[Q26] 计数
来源：http://hz.nwbrower.top/gtkjuwwyuw.html

SELECT COUNT(*) FROM users;
来源：http://hz.dashuyun.cn/gtuymuoubw.html

[Q27] 条件计数
来源：http://hz.0kj1m.cn/gtlywttttx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.aizwys.cn/gtdedskesy.html

[Q28] 求和与平均
来源：http://hz.guowangkeji.top/gtzesjuxkz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.9152youxi.cn/gtelfyytff.html

[Q29] 最大最小值
来源：http://hz.gaohongyu789.top/gtpztnocrz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.0kj1m.cn/gtrhflykyp.html

[Q30] 分组统计
来源：http://hz.zhoulong.xyz/gtprmubabu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.xylfe.cn/gtejkpcvwd.html

[Q31] 分组后过滤
来源：http://hz.shanyushiyangkeji.top/gtwzdzcsav.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.dashuyun.cn/gttylthmqi.html

[Q32] 分组拼接字符串
来源：http://hz.sweek.top/gtrtaskejl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtfhzhhoxl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.hongshengwenyu.top/gttbwscmwh.html

[Q33] 多列分组
来源：http://hz.redwolf501.top/gtgbtebngn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shangyingyoupin.top/gtxvqimssf.html

[Q34] 每组取第一条
来源：http://hz.yueranfly.top/gtrqwafoir.html

SELECT * FROM (
来源：http://hz.c1oappe.top/gtqflktfxb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tianlin.xyz/gtxyvejhyj.html

) t WHERE rn = 1;
来源：http://hz.zhijiandao.cn/gtxfoqlojv.html

[Q35] 内连接
来源：http://hz.bjfxy.top/gtjlxvfujz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhijiandao.cn/gtkjeqdxiy.html

[Q36] 左连接
来源：http://hz.ppjwa.cn/gthesdying.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cqqwz.cn/gtecoodlux.html

[Q37] 右连接
来源：http://hz.zhengqikj.top/gtbppvfrta.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.pengpengdd.cyou/gtzauqghbw.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.hammf.cn/gtkazmwnpd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.0kj1m.cn/gtnzbhyyki.html

[Q39] 自连接（查上下级）
来源：http://hz.hnxiangtu.top/gtlwwjxace.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.quarkkingdee.top/gtycnmjaty.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.jianghu66.top/gtjpepeetd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hammf.cn/gtewnrisms.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yvedp.cn/gtkslaeelf.html

[Q41] 多表连接
来源：http://hz.havefunace.top/gtqeakiqzo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.chenjidiqi.icu/gtvrtngess.html

JOIN users u ON u.id = o.user_id
来源：http://hz.xingfuxueyuan.xyz/gtsoykzfnf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.jinqigfzy.top/gtougfgqrq.html

[Q42] 连接条件附加过滤
来源：http://hz.redwolf501.top/gtxigbmkyk.html

SELECT u.name, o.amount FROM users u
来源：http://hz.nanxinkj.top/gtolfiljhv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jlsjyb.cn/gtmrdhhqgq.html

[Q43] 标量子查询
来源：http://hz.aibaodan.cn/gtrfmknhfu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.shangyingyoupin.top/gtlunpejrh.html

[Q44] IN 子查询
来源：http://hz.shzxlz.cn/gtygbqufko.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.gaohongyu789.top/gtbsknkicp.html

[Q45] EXISTS 判断存在
来源：http://hz.guannengcc.top/gtvroltduy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yanxiufei.cn/gtythykclo.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.316326.xyz/gtsstclgei.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nwbrower.top/gtrgcfgwte.html

[Q47] 与平均值比较
来源：http://hz.chenjidiqi.icu/gtuxmmgjpz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.daxiang520.top/gtqwkysjiz.html

[Q48] CTE 公用表表达式
来源：http://hz.hongshengwenyu.top/gtuswbqjur.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.birdmap.top/gtxxaprhya.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhaomingkeji.xyz/gtjgtibmpa.html

[Q49] 更新单行
来源：http://hz.hywenlv.cn/gtpxzzpnof.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shanyushiyangkeji.top/gtzavwmpkv.html

[Q50] 批量更新
来源：http://hz.shanyushiyangkeji.top/gtepccddpx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.vqdsnc.cn/gtfvbhnppf.html

[Q51] 用子查询更新
来源：http://hz.guowangkeji.top/gtweiddiqp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.aizwys.cn/gtbucsutcv.html

[Q52] 删除指定行
来源：http://hz.nwbrower.top/gtxkoyvham.html

DELETE FROM users WHERE id = 10;
来源：http://hz.gaohongyu789.top/gtmmocrayq.html

[Q53] 按条件删除
来源：http://hz.jiagoushi.top/gtuzogundh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xingfuxueyuan.xyz/gtimwshjft.html

[Q54] 清空表
来源：http://hz.fengsongda.top/gtrwwdrdyh.html

TRUNCATE TABLE logs;
来源：http://hz.aibaodan.cn/gtuyvtbgji.html

[Q55] 排名（并列占位）
来源：http://hz.zhiwuduotai.top/gtndowtoxf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cashguo.top/gtmzjoabbr.html

[Q56] 密集排名（并列不占位）
来源：http://hz.quarkkingdee.top/gtuwraivmh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.52xcode.cn/gtepykliib.html

[Q57] 行号
来源：http://hz.birdmap.top/gtkigsxgws.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.fengsongda.top/gtmgecwczm.html

[Q58] 累计求和
来源：http://hz.c1oappe.top/gtvajhzkgl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.daxiang520.top/gtualkhllb.html

[Q59] 分组内累计
来源：http://hz.kuanghao11.cn/gtqovlieml.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinyuanbaomall.cn/gtsojgsmlc.html

[Q60] 取上一行 / 下一行
来源：http://hz.tianlin.xyz/gtqpoogopb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cdnleiting.top/gtxuxunvyo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gtfbwgqksr.html

[Q61] 移动平均
来源：http://hz.ppjwa.cn/gtdfuoetcg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dianchejie.cn/gtkyslddmp.html

[Q62] 分组占比
来源：http://hz.jiagoushi.top/gtvpzbfpoe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yanxiufei.cn/gttxbnkdxl.html

[Q63] 开启事务
来源：http://hz.yj20258888.top/gtthjssxcl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yvedp.cn/gtquyolbsx.html

[Q64] 提交事务
来源：http://hz.0kj1m.cn/gtqqddgrlk.html

COMMIT;
来源：http://hz.yj20258888.top/gtwyexmive.html

[Q65] 回滚事务
来源：http://hz.jlsjyb.cn/gtwxdepmmj.html

ROLLBACK;
来源：http://hz.jyoumei.cn/gtntzmpypv.html

[Q66] 行锁查询
来源：http://hz.hammf.cn/gtkpowbtwt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhoulong.xyz/gtyzatnfzk.html

[Q67] 设置隔离级别
来源：http://hz.cqqwz.cn/gtewjgllri.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xinyue.icu/gtjlymasvj.html

[Q68] 保存点
来源：http://hz.fengsongda.top/gttnfwusog.html

SAVEPOINT sp1;
来源：http://hz.sxryk.cn/gtnzcygsep.html

ROLLBACK TO sp1;
来源：http://hz.zycfv.cn/gthnhyafqd.html

[Q69] 查看执行计划
来源：http://hz.wangshuangyany.cn/gtcsvdjtif.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sweek.top/gtehxugknd.html

[Q70] 更新统计信息
来源：http://hz.52xcode.cn/gtsfpewkze.html

ANALYZE TABLE users;
来源：http://hz.jinghuilouyu.cn/gtckdpuddj.html

[Q71] 查看建表语句
来源：http://hz.wangdashe.top/gtzfrhzyao.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenzaomai.com/gtjhytafpw.html

[Q72] 查看索引
来源：http://hz.zhijiandao.cn/gtbaxczmie.html

SHOW INDEX FROM users;
来源：http://hz.kuanghao11.cn/gtrgzwpleu.html

[Q73] 查看表状态
来源：http://hz.yj202588.top/gtzyqiaufw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yvedp.cn/gtsxgfkdch.html

[Q74] 强制使用索引
来源：http://hz.yonumen.top/gtkqukpklm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.havefunace.top/gtdpnnptbp.html

[Q75] 日期格式化
来源：http://hz.yvedp.cn/gtzxvghzwj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zdqjudy.top/gtdkvhtavi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.mhx1999.top/gtcqqmolzy.html

[Q76] 按天统计
来源：http://hz.guowangkeji.top/gtnhwzwgbf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zycfv.cn/gtqcxywqvx.html

[Q77] 时间加减
来源：http://hz.nwbrower.top/gtiywbinim.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.mhx1999.top/gtvejyzeoo.html

[Q78] 当前时间
来源：http://hz.smart0.xyz/gtxblsksgs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgfzy.top/gtcqwpytqk.html

[Q79] 字符串拼接
来源：http://hz.fzhhl.top/gtiyekohcl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shzxlz.cn/gtggdrowfu.html

[Q80] 字符串截取
来源：http://hz.quarkkingdee.top/gtuvptqjqf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhongyouzk.top/gtppmmmkay.html

[Q81] 字符串替换
来源：http://hz.daxiang520.top/gtrdlhdgeo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ehwqpu.com/gtwaqfzbij.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigfzy.top/gtipwwvpjf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinyuanbaomall.cn/gtwrehrkkf.html

[Q83] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtcorxhhwk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.birdmap.top/gtewxajzxs.html

[Q84] 去除首尾空格
来源：http://hz.shzxlz.cn/gtczhzwctg.html

SELECT TRIM(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtgkyihkek.html

[Q85] 数值取整
来源：http://hz.zhengqikj.top/gtggmkmoqq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigfzy.top/gtaiqxvqmv.html

[Q86] 读取 JSON 字段
来源：http://hz.nanxuanxn.top/gtkzslfxhv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenzaomai.com/gtbdiiftqa.html

[Q87] JSON 字段做条件
来源：http://hz.gaohongyu789.top/gtwyqpgxwe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cheryme.top/gtohjtdyve.html

[Q88] 行转列（条件聚合）
来源：http://hz.dashuyun.cn/gtzktekjds.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ywan-chungtsiang.top/gtjcgybzyu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.mhx1999.top/gtgygjyeid.html

[Q89] 判断表是否存在
来源：http://hz.yanxiufei.cn/gttdmadbhl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.wangshuangyany.cn/gtjgnbyila.html

[Q90] 生成序号列
来源：http://hz.xinyue.icu/gtqizwhzbc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hysaishi.cn/gtbyearhie.html

================================================================================
来源：http://hz.ydzc1.top/gtcpfvqxib.html

R. Bash 专题
来源：http://hz.tanke756.top/gtydgwprzg.html

================================================================================
来源：http://hz.shuidangran.top/gtglvgncho.html

[R01] shebang 与严格模式
来源：http://hz.ydzc1.top/gttrdmflmx.html

#!/usr/bin/env bash
来源：http://hz.jiagoushi.top/gtfmfzjzsl.html

set -euo pipefail
来源：http://hz.zhijiandao.cn/gtkjhcfkxh.html

[R02] 变量赋值与使用
来源：http://hz.nanxinkj.top/gtrpiqygta.html

name="Tom"; echo "$name"
来源：http://hz.jqgufenzy.top/gthrsbfijb.html

[R03] 只读变量
来源：http://hz.feifeiyinyue.top/gtfetwsucd.html

readonly PI=3.14
来源：http://hz.yuxming.cn/gtxykbkuql.html

[R04] 位置参数
来源：http://hz.quarkkingdee.top/gtfzeagpmh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258.top/gtqyjznoim.html

[R05] 参数默认值
来源：http://hz.zhengqikj.top/gtticyakbg.html

name="${1:-default}"
来源：http://hz.yueranfly.top/gtexikihyp.html

[R06] 判断命令是否存在
来源：http://hz.cheryme.top/gtqjknklap.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenlongwang.top/gtxcrlmmgm.html

[R07] if 判断文件
来源：http://hz.yj20258.top/gtkizmephi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shanyushiyangtech.top/gttsqsrdwe.html

[R08] 数值比较
来源：http://hz.yongpay.top/gtfrytfqkz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhongyouzk.top/gtbrlhlauu.html

[R09] 字符串比较
来源：http://hz.cheryme.top/gtjfqhauwm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cdnleiting.top/gtoxuthsbt.html

[R10] 正则匹配
来源：http://hz.zhiwuduotai.top/gttdmnluha.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ydjk.org.cn/gtqwjhegal.html

[R11] case 多分支
来源：http://hz.zhaomingkeji.xyz/gtcvjbjtkb.html

case "$1" in
来源：http://hz.vqdsnc.cn/gtmeakaqcq.html

start) echo "启动" ;;
来源：http://hz.xingfuxueyuan.xyz/gtvzefyhmu.html

stop)  echo "停止" ;;
来源：http://hz.andypj.xyz/gtqosdvzoa.html

*)     echo "未知命令" ;;
来源：http://hz.0kj1m.cn/gtavzxwxmy.html

esac
来源：http://hz.yangfankeji.com/gtpcmyjenc.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gtuugppxgl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jyoumei.cn/gtyobmohfq.html

[R13] for 计数循环
来源：http://hz.daxiang520.top/gtclbcjhlp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xingfuxueyuan.xyz/gtelyjvspl.html

[R14] C 风格 for
来源：http://hz.0kj1m.cn/gtlaoupwde.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xylfe.cn/gtldbpcmju.html

[R15] while 逐行读文件
来源：http://hz.hysaishi.cn/gtyfbiyqqx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nanxinkj.top/gtsitkmuqq.html

[R16] until 等待条件
来源：http://hz.yj20258.top/gtplmwdfkf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yvedp.cn/gthgmmobwo.html

[R17] 数组定义与取值
来源：http://hz.ivvv.top/gtgaijgloh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yvedp.cn/gtcrviehyy.html

[R18] 遍历数组
来源：http://hz.xinyue.icu/gtjyrnpzmz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtvusejrkn.html

[R19] 数组长度
来源：http://hz.hnqzz.top/gtxszwzhpm.html

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtntuhcczc.html

[R20] 关联数组（字典）
来源：http://hz.jinyuanbaomall.cn/gtjcqvahmd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daxiang520.top/gtoshegdnz.html

[R21] 字符串长度
来源：http://hz.yongpay.top/gtvnzkfjgj.html

echo "${#s}"
来源：http://hz.xingfuxueyuan.xyz/gtmmcczzem.html

[R22] 截取子串
来源：http://hz.hammf.cn/gtbharsodl.html

echo "${s:0:5}"
来源：http://hz.yanxiufei.cn/gtqygvvfwd.html

[R23] 字符串替换
来源：http://hz.snrcjt.cn/gtphegeofu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cashguo.top/gtnbkxyxtl.html

[R24] 大小写转换
来源：http://hz.mhx1999.top/gtribapbix.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jyoumei.cn/gtklluhvnn.html

[R25] 去后缀 / 去前缀
来源：http://hz.sysykeji.top/gtffzesfrh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangshuangyany.cn/gtkxushaal.html

[R26] 命令替换
来源：http://hz.ydzc1.top/gtcetsmamb.html

now=$(date +%F); echo "$now"
来源：http://hz.zhaomingkeji.xyz/gtzfajwidx.html

[R27] 算术展开
来源：http://hz.yj20258.top/gtlwweddsv.html

echo $((1 + 2 * 3))
来源：http://hz.hfpthk.cn/gtovyfkxup.html

[R28] 浮点运算
来源：http://hz.yonumen.top/gtjaghrdcw.html

echo "scale=2; 10/3" | bc
来源：http://hz.zycfv.cn/gtmdtwlbgi.html

[R29] 定义函数
来源：http://hz.daxiang520.top/gtgfdgoprb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nanxuanxn.top/gtymnpucgi.html

[R30] 函数返回状态码
来源：http://hz.hnqzz.top/gttfvvbdpe.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hysaishi.cn/gtidxtveej.html

[R31] 局部变量
来源：http://hz.zhengqikj.top/gthehiioha.html

f() { local x=1; echo "$x"; }
来源：http://hz.cdnleiting.top/gtvazpepfb.html

[R32] 参数个数校验
来源：http://hz.zhoulong.xyz/gtzebcqvnb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shangyingyoupin.top/gthapskbxq.html

[R33] 捕获错误并提示行号
来源：http://hz.ydzc1.top/gtpiudyldu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gtbimyuess.html

[R34] 退出时清理
来源：http://hz.cashguo.top/gtmbqxsnbr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gttqbrqkhx.html

[R35] 后台执行并等待
来源：http://hz.hfpthk.cn/gtobkeyhjw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgufenzy.top/gtozunvehr.html

[R36] 并发执行多个任务
来源：http://hz.ybcxt.top/gtbtysolpy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhixingplan.top/gtelssxqei.html

[R37] 把输出赋给变量
来源：http://hz.aizwys.cn/gtjuahftgb.html

files=$(ls -1)
来源：http://hz.cheryme.top/gtlagjzbvm.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gtthexhlhh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.smart0.xyz/gtcigikoii.html

[R39] 重定向标准输出与错误
来源：http://hz.jqgufenzy.top/gtnmnbwvgi.html

cmd > out.log 2>&1
来源：http://hz.pycfn.com/gtdktmtjkz.html

[R40] 追加写日志
来源：http://hz.quarkkingdee.top/gtfwcynunp.html

echo "log" >> out.log
来源：http://hz.dianchejie.cn/gtlegmjyuk.html

[R41] 丢弃输出
来源：http://hz.9152youxi.cn/gtbpwrgitz.html

cmd >/dev/null 2>&1
来源：http://hz.hywenlv.cn/gtjipckpjd.html

[R42] 输入重定向
来源：http://hz.hywenlv.cn/gtlnkgujpy.html

wc -l < a.txt
来源：http://hz.cashguo.top/gtlgpgbgif.html

[R43] 按名字查找文件
来源：http://hz.bjfxy.top/gtwmeompqo.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gttkgxunek.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtyofhbgvm.html

find . -mtime -7 -type f
来源：http://hz.redwolf501.top/gtkskuockz.html

[R45] 批量删除
来源：http://hz.jinghuilouyu.cn/gtdyifszyc.html

find . -name "*.tmp" -delete
来源：http://hz.xingfuxueyuan.xyz/gtfgrhdgwp.html

[R46] 递归替换文件内容
来源：http://hz.fzhhl.top/gtxtlmqziw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hywenlv.cn/gtsfvylbyq.html

[R47] sed 单行替换
来源：http://hz.sufxvd.cn/gtfxqfvlrr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.smart0.xyz/gtqtxvkddz.html

[R48] awk 取指定列
来源：http://hz.52xcode.cn/gtnsljyyoj.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtqcexixmh.html

[R49] awk 带条件
来源：http://hz.gotoacloud.top/gtacwibfnr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.birdmap.top/gtlwsfzrkh.html

[R50] awk 求和
来源：http://hz.xuetiantiany.cn/gtnlnjfcwt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtdkapeshu.html

[R51] 排序去重取前几
来源：http://hz.yueranfly.top/gtquzmegwl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinghuilouyu.cn/gtcvrhmzss.html

[R52] 统计行数
来源：http://hz.birdmap.top/gtcrtxpevk.html

wc -l a.txt
来源：http://hz.52xcode.cn/gtzaajvzzu.html

[R53] 查看文件头与实时尾
来源：http://hz.tanke756.top/gtplpuwxhv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.guowangkeji.top/gtncnpoaeh.html

[R54] 比较两个文件
来源：http://hz.mhx1999.top/gtexocmzry.html

diff a.txt b.txt
来源：http://hz.zhaomingkeji.xyz/gtuhojkcoy.html

[R55] 压缩与解压
来源：http://hz.xinyue.icu/gtexgwnxfd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ehwqpu.com/gttbvguybc.html

[R56] 远程拷贝
来源：http://hz.jlsjyb.cn/gtaqvgqirb.html

scp file user@host:/path/
来源：http://hz.xuanzx.com/gtncgxamgm.html

[R57] 远程执行命令
来源：http://hz.cqqwz.cn/gtnhcxhhwb.html

ssh user@host 'uptime'
来源：http://hz.shuidangran.top/gtitnggrac.html

[R58] 下载文件
来源：http://hz.hfpthk.cn/gtfqolybts.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cqqwz.cn/gtvcicabxj.html

[R59] 发 POST JSON
来源：http://hz.yongpay.top/gtwweqhhuy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yueranfly.top/gtntzgtqko.html

[R60] 只看 HTTP 状态码
来源：http://hz.nwbrower.top/gtyzmrwusn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cqqwz.cn/gtkmnpsisa.html

[R61] 磁盘占用
来源：http://hz.jqgufenzy.top/gtezxsxsxl.html

df -h;  du -sh *
来源：http://hz.guannengcc.top/gtumgaxlip.html

[R62] 找最占空间的文件
来源：http://hz.zhixingplan.top/gtyibhrkwv.html

du -ah . | sort -rh | head -10
来源：http://hz.svipenyu.cn/gtdyvvopib.html

[R63] 内存与进程
来源：http://hz.yvedp.cn/gtwsepjgqt.html

free -h;  ps aux | grep nginx
来源：http://hz.meibo888.top/gtrllbmudy.html

[R64] 结束进程
来源：http://hz.nanxuanxn.top/gtseyperem.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nwbrower.top/gtloqvecob.html

[R65] 查看端口占用
来源：http://hz.sweek.top/gtqavfrahx.html


<!-- 参考信息 -->