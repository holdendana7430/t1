代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hz.quarkkingdee.top/gtrayazxrh.html

[Q11] 一次插入多行
来源：http://hz.zhongyouzk.top/gtwuekfxjp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hz.chenjidiqi.icu/gtbffbuckh.html

[Q12] 插入后取自增 ID
来源：http://hz.nwbrower.top/gtqwblhheb.html

INSERT INTO users (name) VALUES ('C');
来源：http://hz.hnxiangtu.top/gtbmxylxiy.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.daria6918.cn/gtpwsaajke.html

[Q13] 忽略重复插入
来源：http://hz.haohaochexian.top/gtddtsbifw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.havefunace.top/gthtxzylig.html

[Q14] 存在则更新（upsert）
来源：http://hz.vqdsnc.cn/gtskrywqnx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.havefunace.top/gthpxptwba.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hysaishi.cn/gtbqfsuqmf.html

[Q15] 查询全部
来源：http://hz.yuxming.cn/gtuoxzsgrj.html

SELECT * FROM users;
来源：http://hz.nanxinkj.top/gthejjaayn.html

[Q16] 查询指定列
来源：http://hz.daxiang520.top/gtuwxudqdn.html

SELECT id, name FROM users;
来源：http://hz.jinqigufen.top/gtuwwezfjq.html

[Q17] 条件查询
来源：http://hz.ywan-chungtsiang.top/gtrumugram.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.0kj1m.cn/gtganmqwnc.html

[Q18] 模糊匹配
来源：http://hz.zhixingplan.top/gtxibvmdns.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.shzxlz.cn/gtcgqvtjdm.html

[Q19] 范围查询
来源：http://hz.yj202588.top/gtpwzfwnul.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.shanyushiyangtech.top/gttasjspli.html

[Q20] IN 列表
来源：http://hz.kuanghao11.cn/gthbjyqmtr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.sufxvd.cn/gtceycyxzb.html

[Q21] 空值判断
来源：http://hz.9152youxi.cn/gtraxucgfm.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.tian-w.cn/gtyergmnns.html

[Q22] 排序
来源：http://hz.gogol.net.cn/gtwkqggyok.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.snrcjt.cn/gtlltwapsy.html

[Q23] 分页
来源：http://hz.ydjk.org.cn/gtfeyleiot.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.vqdsnc.cn/gtakigpgca.html

[Q24] 去重
来源：http://hz.snrcjt.cn/gtoqahnoib.html

SELECT DISTINCT city FROM users;
来源：http://hz.yj20258.top/gthihoruyu.html

[Q25] 只取前 N 条
来源：http://hz.mhx1999.top/gtxepmqluz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yj20258888.top/gtnzhxmlju.html

[Q26] 计数
来源：http://hz.ybcxt.top/gtvivyvvfk.html

SELECT COUNT(*) FROM users;
来源：http://hz.daxiang520.top/gtguqrocnr.html

[Q27] 条件计数
来源：http://hz.dashuyun.cn/gtsgehwvkj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.316326.xyz/gtakkucxos.html

[Q28] 求和与平均
来源：http://hz.zhaomingkeji.xyz/gtxiitesqf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.ivvv.top/gtqiaqytoj.html

[Q29] 最大最小值
来源：http://hz.birdmap.top/gtuurvdnvd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ivvv.top/gtfzxnelyp.html

[Q30] 分组统计
来源：http://hz.dianchejie.cn/gtbqitjlac.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.guowangkeji.top/gtwgcsepln.html

[Q31] 分组后过滤
来源：http://hz.havefunace.top/gtlvyvliiw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.pengpengdd.cyou/gtvbzanpvm.html

[Q32] 分组拼接字符串
来源：http://hz.dashuyun.cn/gthfxywvwp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.chenzaomai.com/gtbkwfsynz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yj20258888.top/gtvehcqsqs.html

[Q33] 多列分组
来源：http://hz.sweek.top/gtxcjfqmlh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jinyuanbaomall.cn/gtumnzrjxu.html

[Q34] 每组取第一条
来源：http://hz.redwolf501.top/gtywbjghsy.html

SELECT * FROM (
来源：http://hz.52xcode.cn/gtesxuvrma.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.vqdsnc.cn/gtioraiugh.html

) t WHERE rn = 1;
来源：http://hz.yj202588.top/gtgwgyjqst.html

[Q35] 内连接
来源：http://hz.shangyingyoupin.top/gtohgqhkiz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xuanzx.com/gtqsxjstqm.html

[Q36] 左连接
来源：http://hz.fengsongda.top/gtqydoohuz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jqgufenzy.top/gttnsfqroz.html

[Q37] 右连接
来源：http://hz.mhx1999.top/gtagdpnpfv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.quarkkingdee.top/gtvgwvszgp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.ivvv.top/gtxwxbzuut.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.c1oappe.top/gtzxxpbzfx.html

[Q39] 自连接（查上下级）
来源：http://hz.yonumen.top/gtijjopuaz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jqgfzy.top/gtgqmjipyt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.svipenyu.cn/gtjzvtjspg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.c1oappe.top/gtkqqneuwh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.andypj.xyz/gtjrmmubhh.html

[Q41] 多表连接
来源：http://hz.feifeiyinyue.top/gtxspetjcs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hnqzz.top/gtsoynzjan.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ivvv.top/gthqkaicxn.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhoulong.xyz/gtnznbduqe.html

[Q42] 连接条件附加过滤
来源：http://hz.tianlin.xyz/gtqtsktjuy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jqgufenzy.top/gtevslzaxa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ivvv.top/gtssvvlzde.html

[Q43] 标量子查询
来源：http://hz.wangdashe.top/gtssgayfal.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.pycfn.com/gtdvxkoymi.html

[Q44] IN 子查询
来源：http://hz.xziqi.cn/gtofcjxmlu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.feifeiyinyue.top/gtyatpvbwy.html

[Q45] EXISTS 判断存在
来源：http://hz.jinqigufen.top/gthproqdfs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhijiandao.cn/gtxcqihaxh.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yvedp.cn/gtqbubsgat.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinghuilouyu.cn/gtnsdozigk.html

[Q47] 与平均值比较
来源：http://hz.jqgfzy.top/gtkyyaoqmm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.zhiwuduotai.top/gtznakglyf.html

[Q48] CTE 公用表表达式
来源：http://hz.cucudq.cn/gtjjnsivxl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guannengcc.top/gtczfuictr.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhoulong.xyz/gtksbqyulc.html

[Q49] 更新单行
来源：http://hz.tian-w.cn/gtuefxgzss.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.tianlin.xyz/gtklxdogrg.html

[Q50] 批量更新
来源：http://hz.chenzaomai.com/gtnaysnajo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yj20258.top/gtijavbriu.html

[Q51] 用子查询更新
来源：http://hz.nanxinkj.top/gtkbvxpqcb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.mhx1999.top/gtijsahivh.html

[Q52] 删除指定行
来源：http://hz.zhixingplan.top/gtjiqjphqi.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtwegnuctr.html

[Q53] 按条件删除
来源：http://hz.jyoumei.cn/gtldamqbfj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ydzc1.top/gtwdqdunsn.html

[Q54] 清空表
来源：http://hz.jianghu66.top/gtazuuzhlq.html

TRUNCATE TABLE logs;
来源：http://hz.meibo888.top/gtvjvxffgy.html

[Q55] 排名（并列占位）
来源：http://hz.xuetiantiany.cn/gtyijctynx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hywenlv.cn/gtdrhbvzsi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.nwbrower.top/gtbnqcrkss.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ehwqpu.com/gtkgcdkjiq.html

[Q57] 行号
来源：http://hz.chenlongwang.top/gtktydhkwc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aibaodan.cn/gtdynvnfla.html

[Q58] 累计求和
来源：http://hz.xingfuxueyuan.xyz/gtwopbfpwe.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.chenzaomai.com/gthgnkwifs.html

[Q59] 分组内累计
来源：http://hz.9152youxi.cn/gtohjmbiae.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.smart0.xyz/gtwnrhabvr.html

[Q60] 取上一行 / 下一行
来源：http://hz.yuanzhike.top/gtnxnpqnrs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gtbsryzzbs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dashuyun.cn/gtoemwabgn.html

[Q61] 移动平均
来源：http://hz.ppjwa.cn/gtepiylegs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cucudq.cn/gtwnkmhfjg.html

[Q62] 分组占比
来源：http://hz.yuanzhike.top/gtjlefxxsw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtgkcsqqsx.html

[Q63] 开启事务
来源：http://hz.yangfankeji.com/gtyqmpgdgq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hongshengwenyu.top/gthcmhyrne.html

[Q64] 提交事务
来源：http://hz.shanyushiyangkeji.top/gtesrpuzce.html

COMMIT;
来源：http://hz.kuanghao11.cn/gtiimnougv.html

[Q65] 回滚事务
来源：http://hz.pycfn.com/gtpnlsycqy.html

ROLLBACK;
来源：http://hz.jinqigfzy.top/gtvewvlags.html

[Q66] 行锁查询
来源：http://hz.bjfxy.top/gtcnsfwuns.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xylfe.cn/gtteqmivtr.html

[Q67] 设置隔离级别
来源：http://hz.jinqigufen.top/gtkvfhctzc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.nwbrower.top/gtlzgjghgd.html

[Q68] 保存点
来源：http://hz.jinghuilouyu.cn/gtheijbffn.html

SAVEPOINT sp1;
来源：http://hz.wangdashe.top/gthgihefmx.html

ROLLBACK TO sp1;
来源：http://hz.hywenlv.cn/gtfgvbmldy.html

[Q69] 查看执行计划
来源：http://hz.tanke756.top/gtjoischxv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xuetiantiany.cn/gtdowswvqg.html

[Q70] 更新统计信息
来源：http://hz.jinqigufen.top/gtisjdebaw.html

ANALYZE TABLE users;
来源：http://hz.dianchejie.cn/gtmbskcmfs.html

[Q71] 查看建表语句
来源：http://hz.wangshuangyany.cn/gtyfbxgrpa.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenjidiqi.icu/gtfglhuxkw.html

[Q72] 查看索引
来源：http://hz.jinghuilouyu.cn/gtatfclplc.html

SHOW INDEX FROM users;
来源：http://hz.jlsjyb.cn/gtouhzcezd.html

[Q73] 查看表状态
来源：http://hz.hongshengwenyu.top/gtdfxzdens.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sufxvd.cn/gtowemwbms.html

[Q74] 强制使用索引
来源：http://hz.feifeiyinyue.top/gteltdrbkk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.snrcjt.cn/gtjwhpvikc.html

[Q75] 日期格式化
来源：http://hz.316326.xyz/gtgqolafuc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gtdbmfpqod.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yvedp.cn/gtflaewdyp.html

[Q76] 按天统计
来源：http://hz.zhongyouzk.top/gtjricmnpc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jlsjyb.cn/gtqqwynqgk.html

[Q77] 时间加减
来源：http://hz.xziqi.cn/gthtevrwtg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhengqikj.top/gtnjsjramj.html

[Q78] 当前时间
来源：http://hz.yueranfly.top/gtjojwazeh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.smart0.xyz/gtatrbtsri.html

[Q79] 字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtjeyvgpjd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zycfv.cn/gtouhddxxg.html

[Q80] 字符串截取
来源：http://hz.jinqigfzy.top/gtgresdeyk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yvedp.cn/gtvkjbjuqe.html

[Q81] 字符串替换
来源：http://hz.shzxlz.cn/gtbasjcqns.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.bjfxy.top/gtjofyxzmr.html

[Q82] 字符长度与字节长度
来源：http://hz.chenzaomai.com/gthgwvwjcp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dianchejie.cn/gtdqsendok.html

[Q83] 大小写转换
来源：http://hz.tianlin.xyz/gtvsbsciif.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtgxwsabtf.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangkeji.top/gtnpsiufsd.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtdchjgtia.html

[Q85] 数值取整
来源：http://hz.ehwqpu.com/gteaucmpai.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gotoacloud.top/gtfudstiux.html

[Q86] 读取 JSON 字段
来源：http://hz.wangdashe.top/gttdiouubb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hongshengwenyu.top/gtjrvzjqxd.html

[Q87] JSON 字段做条件
来源：http://hz.hywenlv.cn/gtkvcftqlq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.gzhubu.top/gthhakswjc.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxuanxn.top/gtqgpibisg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xuetiantiany.cn/gtnrwajtjw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gogol.net.cn/gtdosfvtwy.html

[Q89] 判断表是否存在
来源：http://hz.dashuyun.cn/gtdxallefg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.fengsongda.top/gtwctwfwkk.html

[Q90] 生成序号列
来源：http://hz.cheryme.top/gtrybbhvvz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigufen.top/gtzcmfndwe.html

================================================================================
来源：http://hz.ivvv.top/gtuuonmgfy.html

R. Bash 专题
来源：http://hz.xingfuxueyuan.xyz/gtvpcjfskt.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtlujwddyw.html

[R01] shebang 与严格模式
来源：http://hz.nanxinkj.top/gtyudwmjza.html

#!/usr/bin/env bash
来源：http://hz.sxryk.cn/gtewlumqbq.html

set -euo pipefail
来源：http://hz.pycfn.com/gtpgryfnon.html

[R02] 变量赋值与使用
来源：http://hz.zhixingplan.top/gtpxcwywmc.html

name="Tom"; echo "$name"
来源：http://hz.birdmap.top/gtpbzcmigj.html

[R03] 只读变量
来源：http://hz.sysykeji.top/gtepvsfgiz.html

readonly PI=3.14
来源：http://hz.nanxinkj.top/gtokrvjkja.html

[R04] 位置参数
来源：http://hz.chenzaomai.com/gtwduineuy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.smart0.xyz/gtpgwhuqxg.html

[R05] 参数默认值
来源：http://hz.xingfuxueyuan.xyz/gtudozrwir.html

name="${1:-default}"
来源：http://hz.cucudq.cn/gtmhawrzqm.html

[R06] 判断命令是否存在
来源：http://hz.chenlongwang.top/gtfhopsvba.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtqpkbiwwx.html

[R07] if 判断文件
来源：http://hz.gotoacloud.top/gtdpilhqgy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigfzy.top/gtjeljsvxm.html

[R08] 数值比较
来源：http://hz.9152youxi.cn/gtxthszndu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhixingplan.top/gtwtppituk.html

[R09] 字符串比较
来源：http://hz.0kj1m.cn/gtgyhmyylh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.dianchejie.cn/gtxzvyroyx.html

[R10] 正则匹配
来源：http://hz.hammf.cn/gttchididi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cdnleiting.top/gtftgrstbx.html

[R11] case 多分支
来源：http://hz.hywenlv.cn/gtbntlwfdo.html

case "$1" in
来源：http://hz.yonumen.top/gtrqpxgdlz.html

start) echo "启动" ;;
来源：http://hz.aibaodan.cn/gtcuvjftjh.html

stop)  echo "停止" ;;
来源：http://hz.zhiwuduotai.top/gtkbopjrct.html

*)     echo "未知命令" ;;
来源：http://hz.zhixingplan.top/gtivxhzyya.html

esac
来源：http://hz.hnxiangtu.top/gtwhieambx.html

[R12] for 遍历文件
来源：http://hz.shuidangran.top/gttggnerlo.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtsrwerzzp.html

[R13] for 计数循环
来源：http://hz.sxryk.cn/gtkmrpebjg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cdnleiting.top/gtiwlcocxv.html

[R14] C 风格 for
来源：http://hz.sufxvd.cn/gtbtkfuugs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtcsprrkmt.html

[R15] while 逐行读文件
来源：http://hz.shangyingyoupin.top/gtnjyvwbmx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangdashe.top/gtyxpbokxi.html

[R16] until 等待条件
来源：http://hz.jlsjyb.cn/gtbielvtqy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aizwys.cn/gtxatbtolt.html

[R17] 数组定义与取值
来源：http://hz.zhixingplan.top/gtgwsotyhi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtjqwyqxcx.html

[R18] 遍历数组
来源：http://hz.wangshuangyany.cn/gthbdnfpyg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cheryme.top/gtbyshutom.html

[R19] 数组长度
来源：http://hz.zhiwuduotai.top/gtiqogvgub.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtlylnvdzf.html

[R20] 关联数组（字典）
来源：http://hz.yj20258.top/gtgeichusd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangtech.top/gtwzilbrph.html

[R21] 字符串长度
来源：http://hz.0kj1m.cn/gthbofwsgy.html

echo "${#s}"
来源：http://hz.cucudq.cn/gtzneeaykr.html

[R22] 截取子串
来源：http://hz.svipenyu.cn/gtolvviawt.html

echo "${s:0:5}"
来源：http://hz.gogol.net.cn/gtpzfkifcf.html

[R23] 字符串替换
来源：http://hz.jqgfzy.top/gtgodgpvau.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhijiandao.cn/gtuaurhham.html

[R24] 大小写转换
来源：http://hz.chenzaomai.com/gtwrmyizmi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinqigufen.top/gtfzraxafp.html

[R25] 去后缀 / 去前缀
来源：http://hz.gzhubu.top/gtvtwewgso.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtxvgqfeof.html

[R26] 命令替换
来源：http://hz.guowangkeji.top/gtznabgpel.html

now=$(date +%F); echo "$now"
来源：http://hz.c1oappe.top/gtmfllncaf.html

[R27] 算术展开
来源：http://hz.shangyingyoupin.top/gtmsrvyrba.html

echo $((1 + 2 * 3))
来源：http://hz.tanke756.top/gtzyshxexb.html

[R28] 浮点运算
来源：http://hz.andypj.xyz/gttlvvplhw.html

echo "scale=2; 10/3" | bc
来源：http://hz.meibo888.top/gtnnacursh.html

[R29] 定义函数
来源：http://hz.gotoacloud.top/gtamsuinwj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jiagoushi.top/gtxhyxxtzp.html

[R30] 函数返回状态码
来源：http://hz.cheryme.top/gtvtbvjjth.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hongshengwenyu.top/gtemtvptwe.html

[R31] 局部变量
来源：http://hz.zhengqikj.top/gtdzxixgzp.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtbredkkvf.html

[R32] 参数个数校验
来源：http://hz.0kj1m.cn/gtwcizkmrd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.daxiang520.top/gtezjjgxgi.html

[R33] 捕获错误并提示行号
来源：http://hz.xuanzx.com/gthldfyeqy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dianchejie.cn/gttdyqoyiz.html

[R34] 退出时清理
来源：http://hz.yuanzhike.top/gttofqhbcv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtflvpibmw.html

[R35] 后台执行并等待
来源：http://hz.cdnleiting.top/gtnhzgghym.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuanzx.com/gtdstqwoij.html

[R36] 并发执行多个任务
来源：http://hz.chenzaomai.com/gtzpgweidb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jyoumei.cn/gtvjnkfisx.html

[R37] 把输出赋给变量
来源：http://hz.jqgfzy.top/gtpmltdvsk.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtxguproeb.html

[R38] 管道串联
来源：http://hz.snrcjt.cn/gtkqcwezhj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aizwys.cn/gtvzgttozj.html

[R39] 重定向标准输出与错误
来源：http://hz.havefunace.top/gtnuxukpef.html

cmd > out.log 2>&1
来源：http://hz.c1oappe.top/gturdepnjp.html

[R40] 追加写日志
来源：http://hz.zhaomingkeji.xyz/gtsbgtwgti.html

echo "log" >> out.log
来源：http://hz.dianchejie.cn/gtxvayyhpw.html

[R41] 丢弃输出
来源：http://hz.pengpengdd.cyou/gtzjzyivhg.html

cmd >/dev/null 2>&1
来源：http://hz.cashguo.top/gtedusulrz.html

[R42] 输入重定向
来源：http://hz.kuanghao11.cn/gtytxrnxyl.html

wc -l < a.txt
来源：http://hz.jinghuilouyu.cn/gtsfysbygg.html

[R43] 按名字查找文件
来源：http://hz.jinghuilouyu.cn/gtnfekimsh.html

find . -name "*.log" -type f
来源：http://hz.guowangkeji.top/gtmzbspyxb.html

[R44] 按修改时间查找
来源：http://hz.jqgfzy.top/gtvnxgqmzr.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gtjdjxgyli.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtnzdrcmxo.html

find . -name "*.tmp" -delete
来源：http://hz.vqdsnc.cn/gtrfigehyu.html

[R46] 递归替换文件内容
来源：http://hz.snrcjt.cn/gtkmjkjomr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.aizwys.cn/gtgrzbkoie.html

[R47] sed 单行替换
来源：http://hz.smart0.xyz/gtgerszwke.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shanyushiyangkeji.top/gtozipgwqa.html

[R48] awk 取指定列
来源：http://hz.yonumen.top/gtoxpecvzk.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258.top/gtvnyfxstg.html

[R49] awk 带条件
来源：http://hz.fzhhl.top/gtfbxwtbvc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hysaishi.cn/gtrykhwpfh.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtooijlmpa.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nwbrower.top/gtlervchvc.html

[R51] 排序去重取前几
来源：http://hz.hywenlv.cn/gtmtxkhrig.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.svipenyu.cn/gtqbhdjhjt.html

[R52] 统计行数
来源：http://hz.xinyue.icu/gtvcqvhlsv.html

wc -l a.txt
来源：http://hz.fengsongda.top/gtnxtukowo.html

[R53] 查看文件头与实时尾
来源：http://hz.jlsjyb.cn/gtkthowizn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aizwys.cn/gtmqiwrcam.html

[R54] 比较两个文件
来源：http://hz.cheryme.top/gtgsbcbbcs.html

diff a.txt b.txt
来源：http://hz.ybcxt.top/gtidtgklsj.html

[R55] 压缩与解压
来源：http://hz.bjfxy.top/gtzazljfos.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hfpthk.cn/gtonrkwmkl.html

[R56] 远程拷贝
来源：http://hz.sxryk.cn/gtknqetiox.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gtdziffncl.html

[R57] 远程执行命令
来源：http://hz.sufxvd.cn/gtixfymvrr.html

ssh user@host 'uptime'
来源：http://hz.zhiwuduotai.top/gtjrdgence.html

[R58] 下载文件
来源：http://hz.tanke756.top/gtbugxoxlf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtslqadzpp.html

[R59] 发 POST JSON
来源：http://hz.meibo888.top/gtiwhrikbd.html


<!-- 参考信息 -->