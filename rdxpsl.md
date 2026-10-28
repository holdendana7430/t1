代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://hz.guowangkeji.top/gttrgzkzth.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hz.cdnleiting.top/gtgwqriznt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hz.cucudq.cn/gthrkasgyf.html

[Q15] 查询全部
来源：http://hz.ybcxt.top/gtbnrrzbex.html

SELECT * FROM users;
来源：http://hz.jinghuilouyu.cn/gtfgrhyxbh.html

[Q16] 查询指定列
来源：http://hz.guannengcc.top/gtozzxxfjq.html

SELECT id, name FROM users;
来源：http://hz.cdnleiting.top/gtyussagdi.html

[Q17] 条件查询
来源：http://hz.yangfankeji.com/gtvtwxapjt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.tanke756.top/gtglydhpto.html

[Q18] 模糊匹配
来源：http://hz.yj20258.top/gthvwgnutz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.0kj1m.cn/gtoxdgmnkh.html

[Q19] 范围查询
来源：http://hz.hfpthk.cn/gtojawcbph.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.jlsjyb.cn/gtkdalyvdo.html

[Q20] IN 列表
来源：http://hz.tianlin.xyz/gtenylouzp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.fzhhl.top/gtsjbiszht.html

[Q21] 空值判断
来源：http://hz.ydjk.org.cn/gtuwhtojzn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.shanyushiyangtech.top/gtmzxnnxby.html

[Q22] 排序
来源：http://hz.quarkkingdee.top/gtgsfcunke.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.kuanghao11.cn/gtbydgwkau.html

[Q23] 分页
来源：http://hz.xylfe.cn/gtrdcadiki.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tian-w.cn/gtwmlqejqs.html

[Q24] 去重
来源：http://hz.yuanzhike.top/gtwtlqmmbs.html

SELECT DISTINCT city FROM users;
来源：http://hz.jinqigufen.top/gtjuvsnnmz.html

[Q25] 只取前 N 条
来源：http://hz.jqgufenzy.top/gtdputwjdr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xziqi.cn/gtypoqarfp.html

[Q26] 计数
来源：http://hz.52xcode.cn/gtjmbvegkm.html

SELECT COUNT(*) FROM users;
来源：http://hz.xylfe.cn/gtvawznqtm.html

[Q27] 条件计数
来源：http://hz.jiagoushi.top/gthouvzuqc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.gzhubu.top/gtxgzicijq.html

[Q28] 求和与平均
来源：http://hz.zhiwuduotai.top/gtcrlcujcj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.tian-w.cn/gtkeguxyff.html

[Q29] 最大最小值
来源：http://hz.yj20258888.top/gtnncrpvay.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jinqigfzy.top/gtgkogryxy.html

[Q30] 分组统计
来源：http://hz.jinqigufen.top/gtvwslhfpt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nwbrower.top/gtlxuildnr.html

[Q31] 分组后过滤
来源：http://hz.gogol.net.cn/gtapundxyy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ybcxt.top/gtdwgjmcrf.html

[Q32] 分组拼接字符串
来源：http://hz.havefunace.top/gtexfayppf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.gaohongyu789.top/gtlxxerxso.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shuidangran.top/gtqkgsjmgh.html

[Q33] 多列分组
来源：http://hz.snrcjt.cn/gtpdqugupm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxinkj.top/gtyfgfnfqf.html

[Q34] 每组取第一条
来源：http://hz.zhiwuduotai.top/gtcxjpywib.html

SELECT * FROM (
来源：http://hz.wangdashe.top/gtjwuztpma.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.tanke756.top/gtajydauyu.html

) t WHERE rn = 1;
来源：http://hz.cheryme.top/gtgcebeehd.html

[Q35] 内连接
来源：http://hz.jyoumei.cn/gtjiwgfpjv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.gogol.net.cn/gtynlemxsq.html

[Q36] 左连接
来源：http://hz.tanke756.top/gtuhtejguj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.cdnleiting.top/gtollfyxgn.html

[Q37] 右连接
来源：http://hz.nanxuanxn.top/gtfzkeerir.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.jyoumei.cn/gtypskbbje.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.cheryme.top/gtztuwuohr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.tanke756.top/gtdpshoosp.html

[Q39] 自连接（查上下级）
来源：http://hz.xuetiantiany.cn/gtjfyxqkcl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.xuetiantiany.cn/gtandefusz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ivvv.top/gtprmmgcqa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.xuanzx.com/gtjfboossu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jinyuanbaomall.cn/gtuaycsfun.html

[Q41] 多表连接
来源：http://hz.nanxuanxn.top/gttbyyyree.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.iojbl.cn/gtcwqmerqq.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gthtiuwbht.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.0kj1m.cn/gtshmdpscm.html

[Q42] 连接条件附加过滤
来源：http://hz.tian-w.cn/gthtsdhmbu.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ivvv.top/gtkafzbzxp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.vqdsnc.cn/gtcqtbjodw.html

[Q43] 标量子查询
来源：http://hz.yvedp.cn/gtgzdqxqdg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.jqgfzy.top/gtajttexmm.html

[Q44] IN 子查询
来源：http://hz.feifeiyinyue.top/gtmjjbphbx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.yanxiufei.cn/gtbxmlnugv.html

[Q45] EXISTS 判断存在
来源：http://hz.xingfuxueyuan.xyz/gteovlsxko.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtecdnuerj.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yvedp.cn/gttfmczyhm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtmnpllymk.html

[Q47] 与平均值比较
来源：http://hz.pengpengdd.cyou/gtuwcqhrif.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.shanyushiyangkeji.top/gtzdqiefbn.html

[Q48] CTE 公用表表达式
来源：http://hz.hysaishi.cn/gthoqtssnk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.bjfxy.top/gtmxjhqeoh.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xylfe.cn/gtphkhball.html

[Q49] 更新单行
来源：http://hz.iojbl.cn/gtckpimizo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinghuilouyu.cn/gtolmccihn.html

[Q50] 批量更新
来源：http://hz.jqgfzy.top/gthkdbduwb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jlsjyb.cn/gtzxtymxtg.html

[Q51] 用子查询更新
来源：http://hz.tianlin.xyz/gtuxpenwnn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.vqdsnc.cn/gtyargchpp.html

[Q52] 删除指定行
来源：http://hz.316326.xyz/gtlzunzpmo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yj20258888.top/gtubthrhhg.html

[Q53] 按条件删除
来源：http://hz.shangyingyoupin.top/gtfgyyumuu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hywenlv.cn/gtqzxwaxjy.html

[Q54] 清空表
来源：http://hz.jianghu66.top/gtmqmjtuwz.html

TRUNCATE TABLE logs;
来源：http://hz.mhx1999.top/gtazbqnntc.html

[Q55] 排名（并列占位）
来源：http://hz.sweek.top/gtxnhgacpb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hammf.cn/gtakxeqllx.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hammf.cn/gtihkvvvvw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.gogol.net.cn/gtojqzrquo.html

[Q57] 行号
来源：http://hz.ybcxt.top/gtvpidfjfg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.feifeiyinyue.top/gtxgjdwtor.html

[Q58] 累计求和
来源：http://hz.jqgfzy.top/gtanxgdled.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yueranfly.top/gtrirmxovg.html

[Q59] 分组内累计
来源：http://hz.ybcxt.top/gtlqzjqmwl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhongyouzk.top/gtvftfsbut.html

[Q60] 取上一行 / 下一行
来源：http://hz.shangyingyoupin.top/gtvwflgnhi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sxryk.cn/gtafwobiop.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hammf.cn/gtzkpjycqd.html

[Q61] 移动平均
来源：http://hz.hnqzz.top/gtwfnldztk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.gaohongyu789.top/gthqvgkgks.html

[Q62] 分组占比
来源：http://hz.zhaomingkeji.xyz/gtlttoahra.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shzxlz.cn/gthnmqduob.html

[Q63] 开启事务
来源：http://hz.gzhubu.top/gtlgxspnqf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ywan-chungtsiang.top/gthqnfhmyl.html

[Q64] 提交事务
来源：http://hz.havefunace.top/gtztfviyzh.html

COMMIT;
来源：http://hz.zhixingplan.top/gtptjobcym.html

[Q65] 回滚事务
来源：http://hz.kuanghao11.cn/gtqztkrlac.html

ROLLBACK;
来源：http://hz.gogol.net.cn/gtjkkxrvdq.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtmmueyqui.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.feifeiyinyue.top/gteemgncdx.html

[Q67] 设置隔离级别
来源：http://hz.shanyushiyangtech.top/gtqzdzdjzl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.guowangkeji.top/gtkxuqzccu.html

[Q68] 保存点
来源：http://hz.jqgufenzy.top/gtympooraa.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtuklyluma.html

ROLLBACK TO sp1;
来源：http://hz.zdqjudy.top/gtqdlmnvpv.html

[Q69] 查看执行计划
来源：http://hz.zhengqikj.top/gtgaejgwgg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hysaishi.cn/gtmmxnlkms.html

[Q70] 更新统计信息
来源：http://hz.yuxming.cn/gthbixphwc.html

ANALYZE TABLE users;
来源：http://hz.feifeiyinyue.top/gtczxmvydz.html

[Q71] 查看建表语句
来源：http://hz.316326.xyz/gtvxauxmdy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tian-w.cn/gtyeglfhqb.html

[Q72] 查看索引
来源：http://hz.pengpengdd.cyou/gtnkrcnaga.html

SHOW INDEX FROM users;
来源：http://hz.tanke756.top/gtephnnrvc.html

[Q73] 查看表状态
来源：http://hz.shangyingyoupin.top/gtwffftttc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sufxvd.cn/gtwfxtcbpl.html

[Q74] 强制使用索引
来源：http://hz.redwolf501.top/gtxqdbkddu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj20258888.top/gtegyqsrir.html

[Q75] 日期格式化
来源：http://hz.nwbrower.top/gtuczjsosn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.316326.xyz/gtiqgbzwgn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gogol.net.cn/gtxhtdohsk.html

[Q76] 按天统计
来源：http://hz.zhaomingkeji.xyz/gtsofyibem.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daria6918.cn/gtmtvdvxlv.html

[Q77] 时间加减
来源：http://hz.nanxinkj.top/gtyvrzllqv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.daria6918.cn/gtspinskwm.html

[Q78] 当前时间
来源：http://hz.redwolf501.top/gtxboouqmd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sysykeji.top/gtesucxbuz.html

[Q79] 字符串拼接
来源：http://hz.hfpthk.cn/gtiqmxgufh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cucudq.cn/gtlaoohghl.html

[Q80] 字符串截取
来源：http://hz.fengsongda.top/gtcgybxpku.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yongpay.top/gtgxsuzgzi.html

[Q81] 字符串替换
来源：http://hz.316326.xyz/gttenmmkoq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.zdqjudy.top/gtlofucsfd.html

[Q82] 字符长度与字节长度
来源：http://hz.cqqwz.cn/gtxfwiyubr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dashuyun.cn/gtumwovkkg.html

[Q83] 大小写转换
来源：http://hz.svipenyu.cn/gtsfqszewu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nwbrower.top/gtydpdexgt.html

[Q84] 去除首尾空格
来源：http://hz.gaohongyu789.top/gtakmicixg.html

SELECT TRIM(name) FROM users;
来源：http://hz.ehwqpu.com/gtbdrzlprj.html

[Q85] 数值取整
来源：http://hz.cheryme.top/gtvmdxcvra.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jqgfzy.top/gtzcqulxjo.html

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtcmjtxlaa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jlsjyb.cn/gtvdizcjjh.html

[Q87] JSON 字段做条件
来源：http://hz.gogol.net.cn/gtkznzenzr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.feifeiyinyue.top/gtfakpbpet.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gtcbsaqvmw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xingfuxueyuan.xyz/gttbnjdqyl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhixingplan.top/gtsahsxncn.html

[Q89] 判断表是否存在
来源：http://hz.jinqigufen.top/gtzupkjvxv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.feifeiyinyue.top/gtdowfjdeg.html

[Q90] 生成序号列
来源：http://hz.quarkkingdee.top/gtgqncohiy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fzhhl.top/gtjpfxhjkw.html

================================================================================
来源：http://hz.nanxuanxn.top/gtmyrejfvi.html

R. Bash 专题
来源：http://hz.zhaomingkeji.xyz/gtcuxjgkwi.html

================================================================================
来源：http://hz.fengsongda.top/gtduksuzeu.html

[R01] shebang 与严格模式
来源：http://hz.ydjk.org.cn/gtthvcdwgc.html

#!/usr/bin/env bash
来源：http://hz.zhiwuduotai.top/gtingzsyxn.html

set -euo pipefail
来源：http://hz.xuetiantiany.cn/gtroipaiyu.html

[R02] 变量赋值与使用
来源：http://hz.shzxlz.cn/gtqvisyrxf.html

name="Tom"; echo "$name"
来源：http://hz.vqdsnc.cn/gtfshpthld.html

[R03] 只读变量
来源：http://hz.hammf.cn/gtzlcbuhoc.html

readonly PI=3.14
来源：http://hz.cdnleiting.top/gtajxpldsl.html

[R04] 位置参数
来源：http://hz.gogol.net.cn/gtfanmcxsn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nwbrower.top/gtfhuxoien.html

[R05] 参数默认值
来源：http://hz.meibo888.top/gtobcllpki.html

name="${1:-default}"
来源：http://hz.yvedp.cn/gtufbhfpjd.html

[R06] 判断命令是否存在
来源：http://hz.daria6918.cn/gtvvjpcbif.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ehwqpu.com/gtctwnhhve.html

[R07] if 判断文件
来源：http://hz.gaohongyu789.top/gtfyyoyqkq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cqqwz.cn/gtagejeuyd.html

[R08] 数值比较
来源：http://hz.sufxvd.cn/gtqddqmeih.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xziqi.cn/gtezllegfp.html

[R09] 字符串比较
来源：http://hz.iojbl.cn/gtkrdfsbec.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cucudq.cn/gtyttvbmmi.html

[R10] 正则匹配
来源：http://hz.guowangkeji.top/gtqhdkykeg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shuidangran.top/gtzvwdddwf.html

[R11] case 多分支
来源：http://hz.aizwys.cn/gtthrhiofs.html

case "$1" in
来源：http://hz.guowangkeji.top/gtndspzlsg.html

start) echo "启动" ;;
来源：http://hz.ydjk.org.cn/gtmgqpsawb.html

stop)  echo "停止" ;;
来源：http://hz.xuetiantiany.cn/gtjwzpmqrw.html

*)     echo "未知命令" ;;
来源：http://hz.xziqi.cn/gtfqoeekvw.html

esac
来源：http://hz.c1oappe.top/gtlxkvmagc.html

[R12] for 遍历文件
来源：http://hz.zhoulong.xyz/gtndpkowag.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ivvv.top/gttggosnwn.html

[R13] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtshedkyqz.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hysaishi.cn/gtnoqccpdk.html

[R14] C 风格 for
来源：http://hz.gaohongyu789.top/gtdxvfgkrs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ywan-chungtsiang.top/gtajnpftid.html

[R15] while 逐行读文件
来源：http://hz.dashuyun.cn/gthfqxesea.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xinyue.icu/gtsqbhcnvj.html

[R16] until 等待条件
来源：http://hz.sysykeji.top/gtqwsdtciv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.snrcjt.cn/gtksggjpyh.html

[R17] 数组定义与取值
来源：http://hz.zhongyouzk.top/gtmqhznnxo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.iojbl.cn/gtrdskxume.html

[R18] 遍历数组
来源：http://hz.jqgufenzy.top/gtjxuynxwh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinqigfzy.top/gtfbqowcfd.html

[R19] 数组长度
来源：http://hz.yongpay.top/gtvuxxqwhr.html

echo "${#arr[@]}"
来源：http://hz.jinqigfzy.top/gtvdvzshsh.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtoneqkftl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tianlin.xyz/gteqovrphz.html

[R21] 字符串长度
来源：http://hz.ppjwa.cn/gtmunzgelg.html

echo "${#s}"
来源：http://hz.ydzc1.top/gthxcsausb.html

[R22] 截取子串
来源：http://hz.shzxlz.cn/gtudrnouqy.html

echo "${s:0:5}"
来源：http://hz.chenzaomai.com/gttohlvtdb.html

[R23] 字符串替换
来源：http://hz.hfpthk.cn/gtunzniikp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sufxvd.cn/gtrujszyly.html

[R24] 大小写转换
来源：http://hz.316326.xyz/gtubhrlijl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.havefunace.top/gtlduwvsww.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgfzy.top/gtveqgvnac.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuanzhike.top/gtvwmuncns.html

[R26] 命令替换
来源：http://hz.zhijiandao.cn/gtulrinkiu.html

now=$(date +%F); echo "$now"
来源：http://hz.cucudq.cn/gtlgmakjlq.html

[R27] 算术展开
来源：http://hz.sufxvd.cn/gthtppbbgi.html

echo $((1 + 2 * 3))
来源：http://hz.zhixingplan.top/gtbpfevahn.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gtleklngot.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangtech.top/gtmhuuphxa.html

[R29] 定义函数
来源：http://hz.shanyushiyangtech.top/gtflvrhuyg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.52xcode.cn/gtnwkvwbvq.html

[R30] 函数返回状态码
来源：http://hz.guowangkeji.top/gtexzkmakw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgufenzy.top/gthhavbpew.html

[R31] 局部变量
来源：http://hz.xuetiantiany.cn/gtwjwtvptm.html

f() { local x=1; echo "$x"; }
来源：http://hz.shuidangran.top/gtgzgemlrx.html

[R32] 参数个数校验
来源：http://hz.quarkkingdee.top/gtpgsqxbzn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.snrcjt.cn/gthwxvzhio.html

[R33] 捕获错误并提示行号
来源：http://hz.ppjwa.cn/gtfinnvufv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydjk.org.cn/gtjyboztgo.html

[R34] 退出时清理
来源：http://hz.hywenlv.cn/gtlxcmkvrl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hammf.cn/gtppjzumwt.html

[R35] 后台执行并等待
来源：http://hz.pengpengdd.cyou/gtpuopwdxt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigfzy.top/gtahdhcvra.html

[R36] 并发执行多个任务
来源：http://hz.cucudq.cn/gthhyvagsv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shangyingyoupin.top/gtqpnuijbi.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gtnvmotthe.html

files=$(ls -1)
来源：http://hz.zhijiandao.cn/gtttktmyzq.html

[R38] 管道串联
来源：http://hz.zdqjudy.top/gtqdaqtlty.html

cat a.txt | grep -i error | wc -l
来源：http://hz.meibo888.top/gtntnscbpc.html

[R39] 重定向标准输出与错误
来源：http://hz.vqdsnc.cn/gtqyjynkoi.html

cmd > out.log 2>&1
来源：http://hz.cucudq.cn/gtqwnxbuwh.html

[R40] 追加写日志
来源：http://hz.ydjk.org.cn/gtoftwopey.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtcrtxzrhw.html

[R41] 丢弃输出
来源：http://hz.52xcode.cn/gtcguobczz.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtovmywtvz.html

[R42] 输入重定向
来源：http://hz.cheryme.top/gtptztngbg.html

wc -l < a.txt
来源：http://hz.yongpay.top/gtpglobfqz.html

[R43] 按名字查找文件
来源：http://hz.tanke756.top/gtcyfqnkzo.html

find . -name "*.log" -type f
来源：http://hz.yuanzhike.top/gtuerwfefp.html

[R44] 按修改时间查找
来源：http://hz.hywenlv.cn/gtarvxygfs.html

find . -mtime -7 -type f
来源：http://hz.xingfuxueyuan.xyz/gtgqezqqww.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gtaxquyavh.html

find . -name "*.tmp" -delete
来源：http://hz.zhijiandao.cn/gtwrrkahkq.html

[R46] 递归替换文件内容
来源：http://hz.pengpengdd.cyou/gtdqsvwqgp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ywan-chungtsiang.top/gtgaatmdsy.html

[R47] sed 单行替换
来源：http://hz.feifeiyinyue.top/gtfiupdrsl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangdashe.top/gtdbcsslzo.html

[R48] awk 取指定列
来源：http://hz.shangyingyoupin.top/gtmkdqonvi.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtlqlfzzua.html

[R49] awk 带条件
来源：http://hz.316326.xyz/gtzdfshpsd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuetiantiany.cn/gtnwffkcip.html

[R50] awk 求和
来源：http://hz.gzhubu.top/gthvyirwck.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtfdoprszj.html

[R51] 排序去重取前几
来源：http://hz.ybcxt.top/gtffcfpufz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shangyingyoupin.top/gtilajjszk.html

[R52] 统计行数
来源：http://hz.jinghuilouyu.cn/gttxmvvveg.html

wc -l a.txt
来源：http://hz.guannengcc.top/gtlahrelww.html

[R53] 查看文件头与实时尾
来源：http://hz.jiagoushi.top/gtkwptwrqu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gaohongyu789.top/gtrajwotnq.html

[R54] 比较两个文件
来源：http://hz.52xcode.cn/gthkqbsrfq.html

diff a.txt b.txt
来源：http://hz.dashuyun.cn/gtuzsvkiro.html

[R55] 压缩与解压
来源：http://hz.yj20258888.top/gtnezrgzmt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zdqjudy.top/gtrlgdrdlg.html

[R56] 远程拷贝
来源：http://hz.ehwqpu.com/gtpkjsyfuf.html

scp file user@host:/path/
来源：http://hz.ppjwa.cn/gtqlcsurgp.html

[R57] 远程执行命令
来源：http://hz.aizwys.cn/gtmepedcot.html

ssh user@host 'uptime'
来源：http://hz.yj20258888.top/gtxyfurfzx.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gtdtemfazw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sweek.top/gtmlkohrfu.html

[R59] 发 POST JSON
来源：http://hz.zhoulong.xyz/gtmwcbqdie.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhijiandao.cn/gttllvwuga.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenzaomai.com/gtyyzgrwkm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtjpzsgefj.html

[R61] 磁盘占用
来源：http://hz.yuanzhike.top/gtpadlenzh.html

df -h;  du -sh *
来源：http://hz.jlsjyb.cn/gtflawywoa.html

[R62] 找最占空间的文件
来源：http://hz.smart0.xyz/gtbisftnhh.html

du -ah . | sort -rh | head -10
来源：http://hz.hysaishi.cn/gtsitmmibe.html

[R63] 内存与进程
来源：http://hz.dashuyun.cn/gtstmjadil.html


<!-- 参考信息 -->