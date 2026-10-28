代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.zhijiandao.cn/gtygurasjx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.ywan-chungtsiang.top/gtooohomcg.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.hammf.cn/gtxztckzhp.html

[Q15] 查询全部
来源：http://hz.bjfxy.top/gtyyxkwjbj.html

SELECT * FROM users;
来源：http://hz.birdmap.top/gtqgajzcvm.html

[Q16] 查询指定列
来源：http://hz.havefunace.top/gtzxnszddc.html

SELECT id, name FROM users;
来源：http://hz.0kj1m.cn/gtmldqlhtd.html

[Q17] 条件查询
来源：http://hz.cashguo.top/gtwislakic.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.yj20258888.top/gtlaojohht.html

[Q18] 模糊匹配
来源：http://hz.dianchejie.cn/gthqbkgksv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.hywenlv.cn/gtwdjwmyhc.html

[Q19] 范围查询
来源：http://hz.jyoumei.cn/gtxnivqplo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.andypj.xyz/gtxryrzmsq.html

[Q20] IN 列表
来源：http://hz.hnqzz.top/gtsuoqbcqj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.gzhubu.top/gtpgbfhbmq.html

[Q21] 空值判断
来源：http://hz.zhaomingkeji.xyz/gtplnoolvv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.gzhubu.top/gtjptisleu.html

[Q22] 排序
来源：http://hz.316326.xyz/gtytlhahqx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.xylfe.cn/gtrwrppyxl.html

[Q23] 分页
来源：http://hz.quarkkingdee.top/gtnbmunahz.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.ywan-chungtsiang.top/gthmdwwlvq.html

[Q24] 去重
来源：http://hz.tian-w.cn/gtjryvqlab.html

SELECT DISTINCT city FROM users;
来源：http://hz.dianchejie.cn/gtibzwmtsx.html

[Q25] 只取前 N 条
来源：http://hz.shanyushiyangtech.top/gtjgoowlwj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.gotoacloud.top/gtrhdisjhv.html

[Q26] 计数
来源：http://hz.zhoulong.xyz/gtddfrkznr.html

SELECT COUNT(*) FROM users;
来源：http://hz.zdqjudy.top/gthkpkhytc.html

[Q27] 条件计数
来源：http://hz.hywenlv.cn/gtmqhpdgcf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.cdnleiting.top/gtorskdmxc.html

[Q28] 求和与平均
来源：http://hz.shzxlz.cn/gtpcgthfnc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.shanyushiyangtech.top/gtgnpcqdhc.html

[Q29] 最大最小值
来源：http://hz.zhoulong.xyz/gtejlkkuxa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ydjk.org.cn/gtftwbxocy.html

[Q30] 分组统计
来源：http://hz.gaohongyu789.top/gtupbdoivl.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gtpvnzeebk.html

[Q31] 分组后过滤
来源：http://hz.aibaodan.cn/gtkolslfkv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hongshengwenyu.top/gtydmdlckv.html

[Q32] 分组拼接字符串
来源：http://hz.shanyushiyangtech.top/gtesdyobsa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.jinyuanbaomall.cn/gtvokyhhua.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yvedp.cn/gttvtfwxwu.html

[Q33] 多列分组
来源：http://hz.jlsjyb.cn/gtfbykbkep.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jqgufenzy.top/gtmxhytmak.html

[Q34] 每组取第一条
来源：http://hz.jinyuanbaomall.cn/gtbwdetuxj.html

SELECT * FROM (
来源：http://hz.dashuyun.cn/gtlixxinnp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydzc1.top/gticenvjus.html

) t WHERE rn = 1;
来源：http://hz.yuanzhike.top/gtyrvbwmkw.html

[Q35] 内连接
来源：http://hz.aibaodan.cn/gtocikbjnf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ivvv.top/gtrbotlnhx.html

[Q36] 左连接
来源：http://hz.jyoumei.cn/gtffojhiqq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.jianghu66.top/gtzwujbgpi.html

[Q37] 右连接
来源：http://hz.bjfxy.top/gtsocbjvyt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.xuetiantiany.cn/gtbrwzillz.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.xuetiantiany.cn/gtfdfcgbbp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hywenlv.cn/gtwbqosmtb.html

[Q39] 自连接（查上下级）
来源：http://hz.ydjk.org.cn/gtmtjtoaeh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ydjk.org.cn/gtteqmjggc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtzrliscrv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.zhijiandao.cn/gtopxywmaa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.guannengcc.top/gtwmpkbkat.html

[Q41] 多表连接
来源：http://hz.xuetiantiany.cn/gtppuzkvec.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.havefunace.top/gtghtkdojl.html

JOIN users u ON u.id = o.user_id
来源：http://hz.hongshengwenyu.top/gtmzoilimb.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hysaishi.cn/gtmlcblxvc.html

[Q42] 连接条件附加过滤
来源：http://hz.jiagoushi.top/gttwpuwity.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ehwqpu.com/gtvbejknkq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.hysaishi.cn/gtjgivipqs.html

[Q43] 标量子查询
来源：http://hz.jlsjyb.cn/gtmkfhhtxs.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.hywenlv.cn/gtfhdciftd.html

[Q44] IN 子查询
来源：http://hz.cucudq.cn/gtbqxcpalz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.dashuyun.cn/gtffhvjktv.html

[Q45] EXISTS 判断存在
来源：http://hz.fzhhl.top/gtsihotora.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtszsywwqp.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cdnleiting.top/gteinnojtv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gtoplvrnef.html

[Q47] 与平均值比较
来源：http://hz.xingfuxueyuan.xyz/gtduoxgcuf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.dianchejie.cn/gtzuozihfw.html

[Q48] CTE 公用表表达式
来源：http://hz.bjfxy.top/gtqjvyneri.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhoulong.xyz/gthvhlsmte.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jiagoushi.top/gtfumvzvks.html

[Q49] 更新单行
来源：http://hz.nanxinkj.top/gtnlvgwalo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.aibaodan.cn/gtetynjhru.html

[Q50] 批量更新
来源：http://hz.nanxuanxn.top/gtforkumvl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gogol.net.cn/gtmzgkyxzu.html

[Q51] 用子查询更新
来源：http://hz.zdqjudy.top/gtfzttyjnk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinghuilouyu.cn/gtlamcpyjs.html

[Q52] 删除指定行
来源：http://hz.yuxming.cn/gtacsmsagz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yuxming.cn/gtvxtduagc.html

[Q53] 按条件删除
来源：http://hz.haohaochexian.top/gtnjnvsqkg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj202588.top/gtlmsuymuq.html

[Q54] 清空表
来源：http://hz.zhengqikj.top/gtmnogexhy.html

TRUNCATE TABLE logs;
来源：http://hz.yj202588.top/gtvryggtjt.html

[Q55] 排名（并列占位）
来源：http://hz.zycfv.cn/gtkoxtvkkk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xuanzx.com/gtqlmmlvsl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gtcsxgqrbb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.daria6918.cn/gtfwcughta.html

[Q57] 行号
来源：http://hz.zycfv.cn/gtuzmwlaqg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinqigufen.top/gtusgebcxt.html

[Q58] 累计求和
来源：http://hz.shangyingyoupin.top/gtyazflokl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.guannengcc.top/gtwfiiiruk.html

[Q59] 分组内累计
来源：http://hz.fengsongda.top/gttwclurmq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yj20258.top/gtwmwmcajp.html

[Q60] 取上一行 / 下一行
来源：http://hz.dianchejie.cn/gtmueuupmj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sweek.top/gtjncmlppe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.ppjwa.cn/gtilzqnxib.html

[Q61] 移动平均
来源：http://hz.svipenyu.cn/gtibybpwde.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhongyouzk.top/gtrcdugmwc.html

[Q62] 分组占比
来源：http://hz.nanxuanxn.top/gtdlmhgrdx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.xuanzx.com/gtddzsdgac.html

[Q63] 开启事务
来源：http://hz.xuanzx.com/gtdxuooqqr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sufxvd.cn/gtubkpyfxb.html

[Q64] 提交事务
来源：http://hz.xinyue.icu/gtsieijdoy.html

COMMIT;
来源：http://hz.jinyuanbaomall.cn/gtvbkrwrfa.html

[Q65] 回滚事务
来源：http://hz.yonumen.top/gttphsmztr.html

ROLLBACK;
来源：http://hz.shzxlz.cn/gtjzyiywta.html

[Q66] 行锁查询
来源：http://hz.guowangkeji.top/gtwtbsdmrh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.9152youxi.cn/gtptalvimc.html

[Q67] 设置隔离级别
来源：http://hz.nanxuanxn.top/gtrklzwudf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gtduwplinz.html

[Q68] 保存点
来源：http://hz.yonumen.top/gtrsxsrdkq.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gtomdbmnyi.html

ROLLBACK TO sp1;
来源：http://hz.ydzc1.top/gtmyugumji.html

[Q69] 查看执行计划
来源：http://hz.yonumen.top/gtyosbbjyr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jiagoushi.top/gtopkorgyc.html

[Q70] 更新统计信息
来源：http://hz.hysaishi.cn/gtlshqinbt.html

ANALYZE TABLE users;
来源：http://hz.yj20258888.top/gtkzgpwaps.html

[Q71] 查看建表语句
来源：http://hz.chenlongwang.top/gtcqzunmek.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.smart0.xyz/gtvavmgjtl.html

[Q72] 查看索引
来源：http://hz.zhiwuduotai.top/gtgybabsow.html

SHOW INDEX FROM users;
来源：http://hz.daxiang520.top/gtxrmjfjca.html

[Q73] 查看表状态
来源：http://hz.yangfankeji.com/gtsypsrdxl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydzc1.top/gtqmcqnaol.html

[Q74] 强制使用索引
来源：http://hz.shzxlz.cn/gtsqewxajb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtbrssyfqn.html

[Q75] 日期格式化
来源：http://hz.yuanzhike.top/gtrylonods.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tian-w.cn/gthdpoxfet.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.9152youxi.cn/gtwcliydfg.html

[Q76] 按天统计
来源：http://hz.aibaodan.cn/gtmhzzlbua.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cucudq.cn/gtzheimmxv.html

[Q77] 时间加减
来源：http://hz.yuanzhike.top/gtycegqzrb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.xylfe.cn/gtcytnowoi.html

[Q78] 当前时间
来源：http://hz.xingfuxueyuan.xyz/gtczkjhmmv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigfzy.top/gtvgqjidlb.html

[Q79] 字符串拼接
来源：http://hz.yj20258.top/gtjfzlyzvd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sysykeji.top/gtssgcjbcf.html

[Q80] 字符串截取
来源：http://hz.jianghu66.top/gtsabopxvj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gzhubu.top/gtzztdniqc.html

[Q81] 字符串替换
来源：http://hz.xylfe.cn/gtaxqjkpet.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yuanzhike.top/gtkmarsczx.html

[Q82] 字符长度与字节长度
来源：http://hz.cucudq.cn/gtivcymhts.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhengqikj.top/gtanhhujbk.html

[Q83] 大小写转换
来源：http://hz.sufxvd.cn/gtbdsitpbi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.bjfxy.top/gtadevevye.html

[Q84] 去除首尾空格
来源：http://hz.yuanzhike.top/gtwcldayum.html

SELECT TRIM(name) FROM users;
来源：http://hz.yuxming.cn/gtafhkrkjx.html

[Q85] 数值取整
来源：http://hz.yuanzhike.top/gtebtaxmet.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj202588.top/gtoiwhquby.html

[Q86] 读取 JSON 字段
来源：http://hz.hnxiangtu.top/gtfeyssdpn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xuetiantiany.cn/gtqqiomerb.html

[Q87] JSON 字段做条件
来源：http://hz.c1oappe.top/gtvnawulif.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ybcxt.top/gtjgvkaapf.html

[Q88] 行转列（条件聚合）
来源：http://hz.smart0.xyz/gtgsdsseno.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhijiandao.cn/gtkdprlbaf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangdashe.top/gtszxnmngv.html

[Q89] 判断表是否存在
来源：http://hz.havefunace.top/gttpjqjukb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xuanzx.com/gtayktmwsh.html

[Q90] 生成序号列
来源：http://hz.gzhubu.top/gtkpdthnkk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zdqjudy.top/gtyyrctrnl.html

================================================================================
来源：http://hz.yj20258888.top/gtpagorlgd.html

R. Bash 专题
来源：http://hz.zhijiandao.cn/gttydjwwhq.html

================================================================================
来源：http://hz.ppjwa.cn/gtixqblvqd.html

[R01] shebang 与严格模式
来源：http://hz.yangfankeji.com/gtvctqdhrm.html

#!/usr/bin/env bash
来源：http://hz.ydzc1.top/gtzpucdcbr.html

set -euo pipefail
来源：http://hz.chenjidiqi.icu/gtubcgibkq.html

[R02] 变量赋值与使用
来源：http://hz.snrcjt.cn/gtdrrhkvfa.html

name="Tom"; echo "$name"
来源：http://hz.kuanghao11.cn/gtzvjlrzqw.html

[R03] 只读变量
来源：http://hz.zdqjudy.top/gtzeopgsro.html

readonly PI=3.14
来源：http://hz.zhiwuduotai.top/gtinxhigop.html

[R04] 位置参数
来源：http://hz.ppjwa.cn/gtzjuchict.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jlsjyb.cn/gtlxgarpzh.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtorpwaein.html

name="${1:-default}"
来源：http://hz.ehwqpu.com/gtvrrupyxq.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gtxfkeircd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cqqwz.cn/gtrplpfabq.html

[R07] if 判断文件
来源：http://hz.yangfankeji.com/gtlbgfntoh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tian-w.cn/gtzjqvmmnw.html

[R08] 数值比较
来源：http://hz.fengsongda.top/gtwsvzujst.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.vqdsnc.cn/gtmipyrupl.html

[R09] 字符串比较
来源：http://hz.zhengqikj.top/gtvpfvqhiw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.meibo888.top/gtzkbtseqp.html

[R10] 正则匹配
来源：http://hz.9152youxi.cn/gtotnaibtu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ppjwa.cn/gthronhetj.html

[R11] case 多分支
来源：http://hz.hnqzz.top/gtolhgqsdf.html

case "$1" in
来源：http://hz.feifeiyinyue.top/gtmrifqgsy.html

start) echo "启动" ;;
来源：http://hz.shanyushiyangkeji.top/gtdolcupje.html

stop)  echo "停止" ;;
来源：http://hz.hnxiangtu.top/gtjizfwkqv.html

*)     echo "未知命令" ;;
来源：http://hz.bjfxy.top/gttuznecnn.html

esac
来源：http://hz.xuetiantiany.cn/gtluifglwv.html

[R12] for 遍历文件
来源：http://hz.havefunace.top/gtgygzbgve.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xingfuxueyuan.xyz/gtgpwqnmuc.html

[R13] for 计数循环
来源：http://hz.yongpay.top/gtdzxogwui.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhongyouzk.top/gtgrgykmlb.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtrcqsxzxh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtmwmpelhh.html

[R15] while 逐行读文件
来源：http://hz.sufxvd.cn/gtqxuycknu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.c1oappe.top/gtpfjknclk.html

[R16] until 等待条件
来源：http://hz.sufxvd.cn/gtiekqtuve.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenzaomai.com/gtejawhsef.html

[R17] 数组定义与取值
来源：http://hz.jqgufenzy.top/gtbibhpqjr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nwbrower.top/gtctmdggnf.html

[R18] 遍历数组
来源：http://hz.shangyingyoupin.top/gtdfyvzvlp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hongshengwenyu.top/gttcscdrxk.html

[R19] 数组长度
来源：http://hz.yvedp.cn/gtxxjzovtm.html

echo "${#arr[@]}"
来源：http://hz.andypj.xyz/gtlcqlidnr.html

[R20] 关联数组（字典）
来源：http://hz.aibaodan.cn/gtywximsmt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangtech.top/gtvhjngdai.html

[R21] 字符串长度
来源：http://hz.cdnleiting.top/gtdqxcdoyd.html

echo "${#s}"
来源：http://hz.quarkkingdee.top/gtfyfaqdlp.html

[R22] 截取子串
来源：http://hz.jqgufenzy.top/gtlqqmuusj.html

echo "${s:0:5}"
来源：http://hz.ydzc1.top/gtyddolass.html

[R23] 字符串替换
来源：http://hz.havefunace.top/gtbwygwcwx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gaohongyu789.top/gtfzqjmzpa.html

[R24] 大小写转换
来源：http://hz.smart0.xyz/gtjhtbgoea.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.316326.xyz/gttslmkymk.html

[R25] 去后缀 / 去前缀
来源：http://hz.guowangkeji.top/gtibrkibhb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shanyushiyangtech.top/gtrjitlkyd.html

[R26] 命令替换
来源：http://hz.aibaodan.cn/gthnnqvcjb.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gtmuwkmbou.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gtwbefhldm.html

echo $((1 + 2 * 3))
来源：http://hz.hammf.cn/gthqmmxocn.html

[R28] 浮点运算
来源：http://hz.yangfankeji.com/gtpgzyqfwb.html

echo "scale=2; 10/3" | bc
来源：http://hz.jyoumei.cn/gtzubgxxlm.html

[R29] 定义函数
来源：http://hz.jiagoushi.top/gtryphstxo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuanzhike.top/gttabvmlsa.html

[R30] 函数返回状态码
来源：http://hz.gotoacloud.top/gtqphmxemq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.0kj1m.cn/gtdncwsirt.html

[R31] 局部变量
来源：http://hz.jiagoushi.top/gtlxslhixk.html

f() { local x=1; echo "$x"; }
来源：http://hz.yangfankeji.com/gtguooiplo.html

[R32] 参数个数校验
来源：http://hz.feifeiyinyue.top/gtrofcsdjz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtradmryov.html

[R33] 捕获错误并提示行号
来源：http://hz.guannengcc.top/gtzuvzawpe.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.0kj1m.cn/gtiazycjuh.html

[R34] 退出时清理
来源：http://hz.c1oappe.top/gtlwxydipm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtfermiodj.html

[R35] 后台执行并等待
来源：http://hz.shangyingyoupin.top/gtzaeynkpc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinyuanbaomall.cn/gtahwcioel.html

[R36] 并发执行多个任务
来源：http://hz.yanxiufei.cn/gttetpbtui.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jianghu66.top/gtymrocdyg.html

[R37] 把输出赋给变量
来源：http://hz.yuanzhike.top/gtnxelhevz.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtuotchbiw.html

[R38] 管道串联
来源：http://hz.9152youxi.cn/gthlwjchas.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cqqwz.cn/gtawklcqhz.html

[R39] 重定向标准输出与错误
来源：http://hz.ywan-chungtsiang.top/gtoywozuvq.html

cmd > out.log 2>&1
来源：http://hz.ywan-chungtsiang.top/gtwmxherax.html

[R40] 追加写日志
来源：http://hz.aibaodan.cn/gtnqulwqij.html

echo "log" >> out.log
来源：http://hz.fzhhl.top/gtiiaexidr.html

[R41] 丢弃输出
来源：http://hz.pengpengdd.cyou/gtmylhvixm.html

cmd >/dev/null 2>&1
来源：http://hz.9152youxi.cn/gtnwavqnoi.html

[R42] 输入重定向
来源：http://hz.zhiwuduotai.top/gtchhkvryu.html

wc -l < a.txt
来源：http://hz.zdqjudy.top/gtimsumpcj.html

[R43] 按名字查找文件
来源：http://hz.shzxlz.cn/gtqcvrlybd.html

find . -name "*.log" -type f
来源：http://hz.aibaodan.cn/gtwrmswaiv.html

[R44] 按修改时间查找
来源：http://hz.jqgufenzy.top/gtxxaurlwe.html

find . -mtime -7 -type f
来源：http://hz.yvedp.cn/gtsowlxrqt.html

[R45] 批量删除
来源：http://hz.feifeiyinyue.top/gtojdtgxzb.html

find . -name "*.tmp" -delete
来源：http://hz.daxiang520.top/gtazlerdld.html

[R46] 递归替换文件内容
来源：http://hz.c1oappe.top/gtvgrrzvxe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.bjfxy.top/gtaxxnsffs.html

[R47] sed 单行替换
来源：http://hz.pengpengdd.cyou/gtnasddewi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ywan-chungtsiang.top/gtumwytvir.html

[R48] awk 取指定列
来源：http://hz.hysaishi.cn/gtlnmtyyyh.html

awk '{print $1, $3}' a.txt
来源：http://hz.havefunace.top/gtfnxkqxae.html

[R49] awk 带条件
来源：http://hz.ydjk.org.cn/gtafrnxhae.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gaohongyu789.top/gtjzdbmrsb.html

[R50] awk 求和
来源：http://hz.sysykeji.top/gtvifcreoi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtadvwvzbz.html

[R51] 排序去重取前几
来源：http://hz.yj202588.top/gtblqpjeds.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.0kj1m.cn/gtfayjgkoq.html

[R52] 统计行数
来源：http://hz.zhongyouzk.top/gtmeskaile.html

wc -l a.txt
来源：http://hz.shzxlz.cn/gtrkjnttts.html

[R53] 查看文件头与实时尾
来源：http://hz.zycfv.cn/gtiqzuvduk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhiwuduotai.top/gtzikgoxxh.html

[R54] 比较两个文件
来源：http://hz.xylfe.cn/gtweosglzh.html

diff a.txt b.txt
来源：http://hz.0kj1m.cn/gtcmellvsq.html

[R55] 压缩与解压
来源：http://hz.haohaochexian.top/gtbmntqpwk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yonumen.top/gtwegfcfbw.html

[R56] 远程拷贝
来源：http://hz.smart0.xyz/gthvvcqxbg.html

scp file user@host:/path/
来源：http://hz.pengpengdd.cyou/gtlwypkngj.html

[R57] 远程执行命令
来源：http://hz.dashuyun.cn/gtfuyxvbub.html

ssh user@host 'uptime'
来源：http://hz.xingfuxueyuan.xyz/gtnjfuitvy.html

[R58] 下载文件
来源：http://hz.xylfe.cn/gtvxlfqewe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gzhubu.top/gtvnxoxoev.html

[R59] 发 POST JSON
来源：http://hz.redwolf501.top/gtqzuglerh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pycfn.com/gtcyggbcxa.html

[R60] 只看 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtxpsaljhe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cheryme.top/gtrspqwjge.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtbhjukrfn.html

df -h;  du -sh *
来源：http://hz.gogol.net.cn/gtyfsgxffo.html

[R62] 找最占空间的文件
来源：http://hz.fzhhl.top/gtdbntokom.html

du -ah . | sort -rh | head -10
来源：http://hz.zhijiandao.cn/gtsndusdzz.html

[R63] 内存与进程
来源：http://hz.wangdashe.top/gtyuvgztix.html


<!-- 参考信息 -->