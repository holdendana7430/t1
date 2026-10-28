代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://hz.sxryk.cn/gtwhulddfd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hz.zhaomingkeji.xyz/gtruwetppd.html

[Q13] 忽略重复插入
来源：http://hz.hongshengwenyu.top/gtzaxvxplg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hz.yonumen.top/gtmwtekpjt.html

[Q14] 存在则更新（upsert）
来源：http://hz.yangfankeji.com/gtywevaeyl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.jianghu66.top/gtlcdyaylz.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.shanyushiyangtech.top/gtjvfyipcu.html

[Q15] 查询全部
来源：http://hz.sxryk.cn/gtrrnlnscr.html

SELECT * FROM users;
来源：http://hz.hnxiangtu.top/gtpqrcslzn.html

[Q16] 查询指定列
来源：http://hz.havefunace.top/gtpfiumshj.html

SELECT id, name FROM users;
来源：http://hz.316326.xyz/gtaerdewpb.html

[Q17] 条件查询
来源：http://hz.tian-w.cn/gtsjtuyacc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.mhx1999.top/gtctlyhtxf.html

[Q18] 模糊匹配
来源：http://hz.jianghu66.top/gtonnmcker.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.ydjk.org.cn/gtwrloivig.html

[Q19] 范围查询
来源：http://hz.gogol.net.cn/gtipnsnyuo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.yonumen.top/gtmevhnfyg.html

[Q20] IN 列表
来源：http://hz.redwolf501.top/gtpthhdfni.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.zhiwuduotai.top/gtxjhyinai.html

[Q21] 空值判断
来源：http://hz.tanke756.top/gtztlixtgu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.yuxming.cn/gtrkkujoiu.html

[Q22] 排序
来源：http://hz.yj20258888.top/gthlbkunwj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.iojbl.cn/gthhkvbwcs.html

[Q23] 分页
来源：http://hz.nwbrower.top/gtoqichflt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.chenjidiqi.icu/gtnwnjzige.html

[Q24] 去重
来源：http://hz.0kj1m.cn/gtpmlmrvlu.html

SELECT DISTINCT city FROM users;
来源：http://hz.yuanzhike.top/gtuwtbrlyl.html

[Q25] 只取前 N 条
来源：http://hz.hfpthk.cn/gtuknckkin.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.jinqigfzy.top/gtaatjrynv.html

[Q26] 计数
来源：http://hz.xinyue.icu/gtgbzvhqyj.html

SELECT COUNT(*) FROM users;
来源：http://hz.tanke756.top/gtiseqrwxv.html

[Q27] 条件计数
来源：http://hz.xingfuxueyuan.xyz/gtqmfpyyho.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.mhx1999.top/gtlurfqtzp.html

[Q28] 求和与平均
来源：http://hz.zycfv.cn/gtvvyvyyar.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.dashuyun.cn/gtlndejgol.html

[Q29] 最大最小值
来源：http://hz.mhx1999.top/gtvzsdhawk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yj20258888.top/gtlsbrnulh.html

[Q30] 分组统计
来源：http://hz.jinghuilouyu.cn/gtjwlyclww.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.0kj1m.cn/gtwkrrssoc.html

[Q31] 分组后过滤
来源：http://hz.316326.xyz/gtfazpoxuo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.chenlongwang.top/gtrivjrmuc.html

[Q32] 分组拼接字符串
来源：http://hz.xinyue.icu/gtiazlfejx.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xingfuxueyuan.xyz/gtazmxlmgy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.wangdashe.top/gtpxdernsh.html

[Q33] 多列分组
来源：http://hz.gaohongyu789.top/gtahkhwqhp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.hnqzz.top/gtuqrakvqj.html

[Q34] 每组取第一条
来源：http://hz.nwbrower.top/gtbpwcljdz.html

SELECT * FROM (
来源：http://hz.c1oappe.top/gtdtthbrld.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydjk.org.cn/gtalopscdr.html

) t WHERE rn = 1;
来源：http://hz.ydzc1.top/gtpdsxtrdk.html

[Q35] 内连接
来源：http://hz.9152youxi.cn/gtqpauffes.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.tian-w.cn/gtnmtbbfkc.html

[Q36] 左连接
来源：http://hz.hammf.cn/gttndwzppv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.sxryk.cn/gtmaokowkm.html

[Q37] 右连接
来源：http://hz.xuanzx.com/gtxuryzgxu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.sysykeji.top/gtglyduatn.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.vqdsnc.cn/gtzmcwnety.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hongshengwenyu.top/gtfnvnvzii.html

[Q39] 自连接（查上下级）
来源：http://hz.yj20258.top/gtrnowrpff.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.zhongyouzk.top/gtmihcwkxh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.daxiang520.top/gtoxizikiw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jiagoushi.top/gtzyfrvpei.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangtech.top/gtbqcoqtnv.html

[Q41] 多表连接
来源：http://hz.zhiwuduotai.top/gtiywielpp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jqgufenzy.top/gtfnfnoovo.html

JOIN users u ON u.id = o.user_id
来源：http://hz.nanxuanxn.top/gtcecnnttv.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.smart0.xyz/gtwggnptjd.html

[Q42] 连接条件附加过滤
来源：http://hz.pengpengdd.cyou/gtencxnyqw.html

SELECT u.name, o.amount FROM users u
来源：http://hz.iojbl.cn/gtycnsjonj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hongshengwenyu.top/gthrkphcgr.html

[Q43] 标量子查询
来源：http://hz.yueranfly.top/gtqtfvouvn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cqqwz.cn/gthopnockk.html

[Q44] IN 子查询
来源：http://hz.vqdsnc.cn/gtlkbzwpuj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yongpay.top/gtdmuvkgpd.html

[Q45] EXISTS 判断存在
来源：http://hz.ppjwa.cn/gtwvbxikel.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.svipenyu.cn/gtysotzokn.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtkxaajvmh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yj20258888.top/gtjscywaeu.html

[Q47] 与平均值比较
来源：http://hz.hnqzz.top/gtpegsiruo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.aizwys.cn/gtlrktkfeo.html

[Q48] CTE 公用表表达式
来源：http://hz.nwbrower.top/gtvotjdqxj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.guowangkeji.top/gtxjdzweyi.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.ydjk.org.cn/gtitumgatr.html

[Q49] 更新单行
来源：http://hz.9152youxi.cn/gtkcmqjdyj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnxiangtu.top/gtayqhfncq.html

[Q50] 批量更新
来源：http://hz.chenzaomai.com/gtxgobojic.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.cqqwz.cn/gtrskbwwdq.html

[Q51] 用子查询更新
来源：http://hz.nanxinkj.top/gthsnktzgh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yongpay.top/gtkyzeehnt.html

[Q52] 删除指定行
来源：http://hz.redwolf501.top/gtthfriped.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuanzhike.top/gtfaymqrcp.html

[Q53] 按条件删除
来源：http://hz.havefunace.top/gtnshiczas.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.ehwqpu.com/gtvzcmttaz.html

[Q54] 清空表
来源：http://hz.sweek.top/gtbzizhxei.html

TRUNCATE TABLE logs;
来源：http://hz.shuidangran.top/gtgkxjaobi.html

[Q55] 排名（并列占位）
来源：http://hz.kuanghao11.cn/gtvmypqecj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.cqqwz.cn/gtxkvxfcwo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhongyouzk.top/gtxjuzzmyw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.redwolf501.top/gtxfanttbs.html

[Q57] 行号
来源：http://hz.ppjwa.cn/gtxcjognyi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.snrcjt.cn/gtswljndcq.html

[Q58] 累计求和
来源：http://hz.pengpengdd.cyou/gtzuhpzfxi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.meibo888.top/gtkufuldmw.html

[Q59] 分组内累计
来源：http://hz.yuxming.cn/gtdehoiqdq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yangfankeji.com/gtxjzhqedi.html

[Q60] 取上一行 / 下一行
来源：http://hz.cdnleiting.top/gthctcsomz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258888.top/gttackadja.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ppjwa.cn/gtpytvraam.html

[Q61] 移动平均
来源：http://hz.9152youxi.cn/gtqdrffjdk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.chenlongwang.top/gtrpcxhvcc.html

[Q62] 分组占比
来源：http://hz.quarkkingdee.top/gtcotsdifu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtkfoeennl.html

[Q63] 开启事务
来源：http://hz.pengpengdd.cyou/gtzmkvusyt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hysaishi.cn/gtjupmloyx.html

[Q64] 提交事务
来源：http://hz.fengsongda.top/gtgisfreph.html

COMMIT;
来源：http://hz.sufxvd.cn/gtfagyixnw.html

[Q65] 回滚事务
来源：http://hz.birdmap.top/gtiwxccnjw.html

ROLLBACK;
来源：http://hz.andypj.xyz/gtbnxizbas.html

[Q66] 行锁查询
来源：http://hz.dianchejie.cn/gtiqjdswha.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.wangshuangyany.cn/gtloehzuml.html

[Q67] 设置隔离级别
来源：http://hz.chenlongwang.top/gtmxdejylq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jyoumei.cn/gtiyantemu.html

[Q68] 保存点
来源：http://hz.nwbrower.top/gtvguzetjo.html

SAVEPOINT sp1;
来源：http://hz.yj20258888.top/gtfjvysnii.html

ROLLBACK TO sp1;
来源：http://hz.fengsongda.top/gtwoychugd.html

[Q69] 查看执行计划
来源：http://hz.yj20258888.top/gtqgwfhivb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fzhhl.top/gtlvxfliuz.html

[Q70] 更新统计信息
来源：http://hz.chenzaomai.com/gtkjnschrf.html

ANALYZE TABLE users;
来源：http://hz.yj202588.top/gtfjkqehjk.html

[Q71] 查看建表语句
来源：http://hz.hywenlv.cn/gtusyajgzn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ydjk.org.cn/gtjsqlyvlp.html

[Q72] 查看索引
来源：http://hz.yonumen.top/gttyggovzw.html

SHOW INDEX FROM users;
来源：http://hz.aibaodan.cn/gtmkmgqlxh.html

[Q73] 查看表状态
来源：http://hz.chenzaomai.com/gtbdekdlff.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gtxupfufum.html

[Q74] 强制使用索引
来源：http://hz.daria6918.cn/gtnwydldua.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.redwolf501.top/gtunubwmjz.html

[Q75] 日期格式化
来源：http://hz.zhengqikj.top/gtkbgdimvo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj202588.top/gtyhgezflb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jyoumei.cn/gthyrzctik.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gtdgqywckj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenzaomai.com/gtceejuriv.html

[Q77] 时间加减
来源：http://hz.yj20258888.top/gtxnvhbjvi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shuidangran.top/gtjetudekh.html

[Q78] 当前时间
来源：http://hz.mhx1999.top/gtdljuwfpq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dianchejie.cn/gtskqyujdc.html

[Q79] 字符串拼接
来源：http://hz.xylfe.cn/gtxckfcabk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pengpengdd.cyou/gtyvmczkfr.html

[Q80] 字符串截取
来源：http://hz.yj20258.top/gtceeolvly.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.mhx1999.top/gtduyjdryj.html

[Q81] 字符串替换
来源：http://hz.ybcxt.top/gtdbkwmatp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jyoumei.cn/gtqshsfzzs.html

[Q82] 字符长度与字节长度
来源：http://hz.c1oappe.top/gtutufheln.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydzc1.top/gtxkvyjwlu.html

[Q83] 大小写转换
来源：http://hz.daxiang520.top/gtikzsmrxv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxuanxn.top/gtudnphpxv.html

[Q84] 去除首尾空格
来源：http://hz.zhongyouzk.top/gtgvrirjrq.html

SELECT TRIM(name) FROM users;
来源：http://hz.hongshengwenyu.top/gttmyjnpsn.html

[Q85] 数值取整
来源：http://hz.wangshuangyany.cn/gtkcbrzhbp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.aizwys.cn/gtlympabxt.html

[Q86] 读取 JSON 字段
来源：http://hz.vqdsnc.cn/gtiaizqume.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.kuanghao11.cn/gtrgpxaelk.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigufen.top/gtonmtbnol.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.iojbl.cn/gtrgrfxzfn.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258.top/gtxjzonqzv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shzxlz.cn/gtgkfnkftr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.aibaodan.cn/gtvhmrxmnb.html

[Q89] 判断表是否存在
来源：http://hz.ivvv.top/gtthpwavnq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yueranfly.top/gtxqebkyts.html

[Q90] 生成序号列
来源：http://hz.jinghuilouyu.cn/gtghynkwiq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hnqzz.top/gtrvsrzcxw.html

================================================================================
来源：http://hz.yuanzhike.top/gtlmxqawih.html

R. Bash 专题
来源：http://hz.guowangkeji.top/gtfrwumwpw.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtovwghvvz.html

[R01] shebang 与严格模式
来源：http://hz.shzxlz.cn/gtyqxjcbvz.html

#!/usr/bin/env bash
来源：http://hz.ivvv.top/gtgseuvdta.html

set -euo pipefail
来源：http://hz.ehwqpu.com/gtlgbdgbwp.html

[R02] 变量赋值与使用
来源：http://hz.jqgfzy.top/gtkhuatutv.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtknjtzdso.html

[R03] 只读变量
来源：http://hz.jyoumei.cn/gtdrrgldus.html

readonly PI=3.14
来源：http://hz.pycfn.com/gttimhqnzf.html

[R04] 位置参数
来源：http://hz.aibaodan.cn/gtefqxgciz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangkeji.top/gtdwrnouqm.html

[R05] 参数默认值
来源：http://hz.yonumen.top/gtktkeshow.html

name="${1:-default}"
来源：http://hz.gzhubu.top/gtppdxnixm.html

[R06] 判断命令是否存在
来源：http://hz.hammf.cn/gtyfmseria.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gthmojcrvs.html

[R07] if 判断文件
来源：http://hz.nanxuanxn.top/gtjjkleohc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.9152youxi.cn/gtuzewcoek.html

[R08] 数值比较
来源：http://hz.jyoumei.cn/gtrcwjbjni.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.chenlongwang.top/gtukacjlkb.html

[R09] 字符串比较
来源：http://hz.guannengcc.top/gtryhirdiw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sxryk.cn/gtvbaskbho.html

[R10] 正则匹配
来源：http://hz.meibo888.top/gtlrvfskfu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tianlin.xyz/gtuareflst.html

[R11] case 多分支
来源：http://hz.52xcode.cn/gtkhnjvqsz.html

case "$1" in
来源：http://hz.smart0.xyz/gtlmxvfpao.html

start) echo "启动" ;;
来源：http://hz.feifeiyinyue.top/gtfvpuewkp.html

stop)  echo "停止" ;;
来源：http://hz.jianghu66.top/gtvowiebcj.html

*)     echo "未知命令" ;;
来源：http://hz.yongpay.top/gttaommibz.html

esac
来源：http://hz.zhiwuduotai.top/gtolxtxqov.html

[R12] for 遍历文件
来源：http://hz.jinyuanbaomall.cn/gtbxwlqoox.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258.top/gtksnuidka.html

[R13] for 计数循环
来源：http://hz.cqqwz.cn/gtslxuyeju.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jianghu66.top/gtwqhzaiqt.html

[R14] C 风格 for
来源：http://hz.jinyuanbaomall.cn/gtkikjtvml.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yongpay.top/gtzkigfzuj.html

[R15] while 逐行读文件
来源：http://hz.gaohongyu789.top/gtjlhrhxan.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yj20258888.top/gtjpncvgxe.html

[R16] until 等待条件
来源：http://hz.hnqzz.top/gtbfhlsqdf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ivvv.top/gtmcehaoug.html

[R17] 数组定义与取值
来源：http://hz.havefunace.top/gthoavvxun.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.c1oappe.top/gtefnnqxxo.html

[R18] 遍历数组
来源：http://hz.xuanzx.com/gtgjdsdtrs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtstxgdmna.html

[R19] 数组长度
来源：http://hz.zhijiandao.cn/gtwwszjlwh.html

echo "${#arr[@]}"
来源：http://hz.hywenlv.cn/gtnikhxmtp.html

[R20] 关联数组（字典）
来源：http://hz.yj20258.top/gtwvsrizbi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.haohaochexian.top/gtvwsgakyn.html

[R21] 字符串长度
来源：http://hz.zdqjudy.top/gtkfaqqicj.html

echo "${#s}"
来源：http://hz.yj20258.top/gttcxxptoj.html

[R22] 截取子串
来源：http://hz.yonumen.top/gtodjxdlgi.html

echo "${s:0:5}"
来源：http://hz.jlsjyb.cn/gtetbduwoa.html

[R23] 字符串替换
来源：http://hz.bjfxy.top/gtgenjawmu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuetiantiany.cn/gtnwyufrpa.html

[R24] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtparrwayq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.52xcode.cn/gtptixvbsx.html

[R25] 去后缀 / 去前缀
来源：http://hz.shanyushiyangkeji.top/gtjwmnycgw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.c1oappe.top/gtxiqxudga.html

[R26] 命令替换
来源：http://hz.shuidangran.top/gtmudfbyaj.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gtoumhgtwf.html

[R27] 算术展开
来源：http://hz.chenlongwang.top/gtknhurdla.html

echo $((1 + 2 * 3))
来源：http://hz.wangdashe.top/gtunyqshiu.html

[R28] 浮点运算
来源：http://hz.sweek.top/gtgtwchcwp.html

echo "scale=2; 10/3" | bc
来源：http://hz.jyoumei.cn/gtgugentwn.html

[R29] 定义函数
来源：http://hz.yvedp.cn/gtwbuspter.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhijiandao.cn/gtbecylwfm.html

[R30] 函数返回状态码
来源：http://hz.yuxming.cn/gtgeaghlfi.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gotoacloud.top/gtjubigwkx.html

[R31] 局部变量
来源：http://hz.zhaomingkeji.xyz/gtlwmxhsly.html

f() { local x=1; echo "$x"; }
来源：http://hz.svipenyu.cn/gtldbqfuvs.html

[R32] 参数个数校验
来源：http://hz.52xcode.cn/gtasindbhs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xylfe.cn/gtcpmcvhra.html

[R33] 捕获错误并提示行号
来源：http://hz.xuanzx.com/gtmfiduatj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.kuanghao11.cn/gtisoqiupi.html

[R34] 退出时清理
来源：http://hz.andypj.xyz/gtuesppxjx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gotoacloud.top/gtlurhunip.html

[R35] 后台执行并等待
来源：http://hz.xinyue.icu/gttmfrdtpy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cashguo.top/gtlyxylyfx.html

[R36] 并发执行多个任务
来源：http://hz.birdmap.top/gtjweizwlr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sysykeji.top/gtvkwpmffs.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gtrzifofze.html

files=$(ls -1)
来源：http://hz.xuanzx.com/gttxqlaoot.html

[R38] 管道串联
来源：http://hz.jinqigfzy.top/gtkglclmsl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtoicbktdu.html

[R39] 重定向标准输出与错误
来源：http://hz.vqdsnc.cn/gtaiyyawgg.html

cmd > out.log 2>&1
来源：http://hz.hnqzz.top/gterfyjgjl.html

[R40] 追加写日志
来源：http://hz.pycfn.com/gtynijycno.html

echo "log" >> out.log
来源：http://hz.yueranfly.top/gtycevtrlw.html

[R41] 丢弃输出
来源：http://hz.zhoulong.xyz/gtfoaiieja.html

cmd >/dev/null 2>&1
来源：http://hz.xuetiantiany.cn/gtamjkbxxc.html

[R42] 输入重定向
来源：http://hz.redwolf501.top/gtcmimnknp.html

wc -l < a.txt
来源：http://hz.ehwqpu.com/gtbeidkhvw.html

[R43] 按名字查找文件
来源：http://hz.jqgufenzy.top/gtadannloh.html

find . -name "*.log" -type f
来源：http://hz.birdmap.top/gtquiogbbt.html

[R44] 按修改时间查找
来源：http://hz.zdqjudy.top/gtmuqrxbfe.html

find . -mtime -7 -type f
来源：http://hz.jqgufenzy.top/gtgpsfsbkb.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtqnwwrfrr.html

find . -name "*.tmp" -delete
来源：http://hz.yj202588.top/gtedznjxth.html

[R46] 递归替换文件内容
来源：http://hz.sweek.top/gtobasiriu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shuidangran.top/gtmztkuzhv.html

[R47] sed 单行替换
来源：http://hz.sufxvd.cn/gtpgiauydi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jlsjyb.cn/gtpgccjzkd.html

[R48] awk 取指定列
来源：http://hz.jinghuilouyu.cn/gtsvnopzaw.html

awk '{print $1, $3}' a.txt
来源：http://hz.dashuyun.cn/gtoehcrpxz.html

[R49] awk 带条件
来源：http://hz.vqdsnc.cn/gtmunwxspy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuetiantiany.cn/gtlslbugdj.html

[R50] awk 求和
来源：http://hz.sysykeji.top/gtnxseqgeb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtvfqtyvvs.html

[R51] 排序去重取前几
来源：http://hz.yuanzhike.top/gtyymwymoy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yuanzhike.top/gtqqalwuss.html

[R52] 统计行数
来源：http://hz.quarkkingdee.top/gtosgehvtv.html

wc -l a.txt
来源：http://hz.yj20258888.top/gtvmyhemca.html

[R53] 查看文件头与实时尾
来源：http://hz.xuanzx.com/gtqwyzfdsf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhiwuduotai.top/gtabmhldhi.html

[R54] 比较两个文件
来源：http://hz.daxiang520.top/gtirrfrsbc.html

diff a.txt b.txt
来源：http://hz.aizwys.cn/gtnkltjffl.html

[R55] 压缩与解压
来源：http://hz.ybcxt.top/gtnndjmzcv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhongyouzk.top/gtmokfbyxd.html

[R56] 远程拷贝
来源：http://hz.zhengqikj.top/gthgcfzybz.html

scp file user@host:/path/
来源：http://hz.iojbl.cn/gtzkqkzbgp.html

[R57] 远程执行命令
来源：http://hz.ydzc1.top/gttqgzryds.html

ssh user@host 'uptime'
来源：http://hz.yangfankeji.com/gtjnjzwjwm.html

[R58] 下载文件
来源：http://hz.cashguo.top/gtrruuyukr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jlsjyb.cn/gtscqhjwkp.html

[R59] 发 POST JSON
来源：http://hz.dianchejie.cn/gtqqrglcyp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.c1oappe.top/gtflpygslu.html

[R60] 只看 HTTP 状态码
来源：http://hz.daxiang520.top/gthbyprgue.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.redwolf501.top/gtxnjermbv.html

[R61] 磁盘占用
来源：http://hz.vqdsnc.cn/gtgkwxoupo.html


<!-- 参考信息 -->