代发 wailian999

SELECT * FROM users;
来源：http://hz.chenzaomai.com/gterttlyre.html

[Q16] 查询指定列
来源：http://hz.snrcjt.cn/gtekmircqs.html

SELECT id, name FROM users;
来源：http://hz.ydzc1.top/gtdgymlxpd.html

[Q17] 条件查询
来源：http://hz.ydjk.org.cn/gtjtuyojlx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hz.jinqigfzy.top/gttzkdwihz.html

[Q18] 模糊匹配
来源：http://hz.guowangkeji.top/gtydcedick.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hz.jlsjyb.cn/gttqbpwhgj.html

[Q19] 范围查询
来源：http://hz.fengsongda.top/gtxlhjgebl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hz.zdqjudy.top/gtkdaggrnr.html

[Q20] IN 列表
来源：http://hz.xuetiantiany.cn/gtigtorawq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hz.shanyushiyangtech.top/gtdervzcpk.html

[Q21] 空值判断
来源：http://hz.jinghuilouyu.cn/gtnulvlvwr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.dianchejie.cn/gtbkjywjyl.html

[Q22] 排序
来源：http://hz.jinqigfzy.top/gteecgypta.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.yj20258888.top/gtrzqbneup.html

[Q23] 分页
来源：http://hz.meibo888.top/gtmnennwzq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.gaohongyu789.top/gtleboklcf.html

[Q24] 去重
来源：http://hz.52xcode.cn/gtpdbzwukd.html

SELECT DISTINCT city FROM users;
来源：http://hz.zhengqikj.top/gtiwricwpv.html

[Q25] 只取前 N 条
来源：http://hz.zhongyouzk.top/gtzsenckmf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xuanzx.com/gtdobwipgx.html

[Q26] 计数
来源：http://hz.jinyuanbaomall.cn/gteemwbslx.html

SELECT COUNT(*) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtmqerlwyy.html

[Q27] 条件计数
来源：http://hz.havefunace.top/gtfrautcxg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.shanyushiyangtech.top/gtiswyslxj.html

[Q28] 求和与平均
来源：http://hz.jiagoushi.top/gtyrvfgnrv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.zycfv.cn/gtrttxkvqh.html

[Q29] 最大最小值
来源：http://hz.xziqi.cn/gtazcaranl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.jqgfzy.top/gtcxshsrly.html

[Q30] 分组统计
来源：http://hz.hnqzz.top/gtqdonxdsd.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtgtzuuadf.html

[Q31] 分组后过滤
来源：http://hz.xziqi.cn/gtzwrglvum.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.smart0.xyz/gtjasfvxat.html

[Q32] 分组拼接字符串
来源：http://hz.jinyuanbaomall.cn/gtiqtmvpzh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.yj20258888.top/gtcugwtooi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cucudq.cn/gtyuwrisos.html

[Q33] 多列分组
来源：http://hz.havefunace.top/gtlrnluseo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.haohaochexian.top/gtwxoqqpiw.html

[Q34] 每组取第一条
来源：http://hz.yongpay.top/gtyzuhhpxa.html

SELECT * FROM (
来源：http://hz.xziqi.cn/gtgsptbbbj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.316326.xyz/gtmtwsygun.html

) t WHERE rn = 1;
来源：http://hz.haohaochexian.top/gteyxnicjh.html

[Q35] 内连接
来源：http://hz.cucudq.cn/gtyowkgoji.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.sysykeji.top/gtexnlfnke.html

[Q36] 左连接
来源：http://hz.52xcode.cn/gtnhwubjxw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhaomingkeji.xyz/gtvsrazkfs.html

[Q37] 右连接
来源：http://hz.dashuyun.cn/gtgholevka.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hnxiangtu.top/gtasjfsvlo.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shuidangran.top/gtadplgrlh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shangyingyoupin.top/gtwktmysde.html

[Q39] 自连接（查上下级）
来源：http://hz.ydjk.org.cn/gtevwucefc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jinqigfzy.top/gtpewoojdk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.aibaodan.cn/gtiqcduvef.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.daria6918.cn/gtwwfhngri.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.xuetiantiany.cn/gtvbbzoxqt.html

[Q41] 多表连接
来源：http://hz.shanyushiyangtech.top/gtkzitafwr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jinghuilouyu.cn/gtdrwyebvt.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhengqikj.top/gtpwxwkfia.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.bjfxy.top/gtuyagglxp.html

[Q42] 连接条件附加过滤
来源：http://hz.zhoulong.xyz/gtdisjsedc.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zdqjudy.top/gtubuvmkoz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.0kj1m.cn/gtwxpwvtxa.html

[Q43] 标量子查询
来源：http://hz.zdqjudy.top/gtultsimnj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhijiandao.cn/gtpmlgxlik.html

[Q44] IN 子查询
来源：http://hz.zhixingplan.top/gtkxkwokre.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shangyingyoupin.top/gtkctcxmsg.html

[Q45] EXISTS 判断存在
来源：http://hz.shangyingyoupin.top/gtsgjvdtin.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.haohaochexian.top/gtzncfabia.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cdnleiting.top/gtgafmbzcb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhoulong.xyz/gtzwuldfvz.html

[Q47] 与平均值比较
来源：http://hz.xingfuxueyuan.xyz/gtwncfwgea.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.meibo888.top/gtoqkirays.html

[Q48] CTE 公用表表达式
来源：http://hz.zhaomingkeji.xyz/gtdndklfgx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhoulong.xyz/gtorocxock.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.shzxlz.cn/gtqpkuieqz.html

[Q49] 更新单行
来源：http://hz.yonumen.top/gtrqimfihv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangdashe.top/gtinzwoqvs.html

[Q50] 批量更新
来源：http://hz.chenjidiqi.icu/gtfvedpssz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ivvv.top/gtbageskpk.html

[Q51] 用子查询更新
来源：http://hz.xingfuxueyuan.xyz/gtjhpdytfv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hammf.cn/gtkcymkcoo.html

[Q52] 删除指定行
来源：http://hz.tian-w.cn/gtywqbmrix.html

DELETE FROM users WHERE id = 10;
来源：http://hz.tianlin.xyz/gtroncopqc.html

[Q53] 按条件删除
来源：http://hz.nwbrower.top/gtupwqdvle.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.daxiang520.top/gteqjjfhkc.html

[Q54] 清空表
来源：http://hz.hammf.cn/gtjzsuqylb.html

TRUNCATE TABLE logs;
来源：http://hz.zhijiandao.cn/gtxphehcow.html

[Q55] 排名（并列占位）
来源：http://hz.jqgufenzy.top/gtqtycnaep.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.0kj1m.cn/gtensnwcpj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zdqjudy.top/gtbckwnhlm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sweek.top/gtyhagjuzf.html

[Q57] 行号
来源：http://hz.sxryk.cn/gtfrowrnrw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.snrcjt.cn/gtanrquyub.html

[Q58] 累计求和
来源：http://hz.iojbl.cn/gtuslakdut.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jqgfzy.top/gtydcfhfdn.html

[Q59] 分组内累计
来源：http://hz.jinghuilouyu.cn/gtjoiuwggi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yvedp.cn/gtphsbyxpg.html

[Q60] 取上一行 / 下一行
来源：http://hz.fzhhl.top/gthrrgdbgj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.316326.xyz/gtjzcubxoa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gotoacloud.top/gtccnqhqcy.html

[Q61] 移动平均
来源：http://hz.yj20258888.top/gttkirdose.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.pycfn.com/gtwytitgss.html

[Q62] 分组占比
来源：http://hz.tanke756.top/gtrndylpug.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.sweek.top/gthnnmucim.html

[Q63] 开启事务
来源：http://hz.ydjk.org.cn/gtmjuqvhfd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.redwolf501.top/gtkpqgrfeh.html

[Q64] 提交事务
来源：http://hz.jyoumei.cn/gtdrcbrmwq.html

COMMIT;
来源：http://hz.cucudq.cn/gtyjxfscgw.html

[Q65] 回滚事务
来源：http://hz.kuanghao11.cn/gtmggixvms.html

ROLLBACK;
来源：http://hz.svipenyu.cn/gtqzpvuwrx.html

[Q66] 行锁查询
来源：http://hz.haohaochexian.top/gtncyteeja.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yongpay.top/gtpjivqmeu.html

[Q67] 设置隔离级别
来源：http://hz.c1oappe.top/gticpyfvqg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.quarkkingdee.top/gtedtfhhpe.html

[Q68] 保存点
来源：http://hz.pengpengdd.cyou/gtdefqnbqc.html

SAVEPOINT sp1;
来源：http://hz.316326.xyz/gtffavkxfd.html

ROLLBACK TO sp1;
来源：http://hz.jinqigfzy.top/gttdmxwehh.html

[Q69] 查看执行计划
来源：http://hz.shzxlz.cn/gtafuajkej.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tanke756.top/gtuwjvgrcj.html

[Q70] 更新统计信息
来源：http://hz.yj20258.top/gtthgmgwvq.html

ANALYZE TABLE users;
来源：http://hz.yonumen.top/gtmzymvqag.html

[Q71] 查看建表语句
来源：http://hz.xuanzx.com/gtlyuboopl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhaomingkeji.xyz/gtylwdlmde.html

[Q72] 查看索引
来源：http://hz.hnqzz.top/gtxgnikzgk.html

SHOW INDEX FROM users;
来源：http://hz.hywenlv.cn/gtpvipxmge.html

[Q73] 查看表状态
来源：http://hz.sxryk.cn/gtuwxtaedg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hammf.cn/gtrvqwqjik.html

[Q74] 强制使用索引
来源：http://hz.gotoacloud.top/gtaftmtink.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.316326.xyz/gttxdqrbbz.html

[Q75] 日期格式化
来源：http://hz.xinyue.icu/gtsucrziaf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yuanzhike.top/gtrhuqpqtp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtbiifnayb.html

[Q76] 按天统计
来源：http://hz.jinyuanbaomall.cn/gtdbogszxk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xziqi.cn/gtwbvgiqza.html

[Q77] 时间加减
来源：http://hz.xylfe.cn/gtzlfscfdt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinghuilouyu.cn/gtbwmclfwz.html

[Q78] 当前时间
来源：http://hz.yonumen.top/gtfztevyqr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shanyushiyangkeji.top/gtmnvxeufg.html

[Q79] 字符串拼接
来源：http://hz.sweek.top/gtobmejplt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenzaomai.com/gtahxnrxbd.html

[Q80] 字符串截取
来源：http://hz.jinqigfzy.top/gtafmflodx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtdwqkbolx.html

[Q81] 字符串替换
来源：http://hz.guowangkeji.top/gtijtooykm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shuidangran.top/gtclfhcght.html

[Q82] 字符长度与字节长度
来源：http://hz.shanyushiyangtech.top/gtzcoyjzix.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gtibgpbltt.html

[Q83] 大小写转换
来源：http://hz.jqgfzy.top/gtfeynyybf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gogol.net.cn/gtybkjhykq.html

[Q84] 去除首尾空格
来源：http://hz.gogol.net.cn/gtxuadnncg.html

SELECT TRIM(name) FROM users;
来源：http://hz.kuanghao11.cn/gtyjkcrlgt.html

[Q85] 数值取整
来源：http://hz.ivvv.top/gtayafrxmq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydzc1.top/gtvrrkwdrw.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gthninonlp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.ydzc1.top/gtvawbseoe.html

[Q87] JSON 字段做条件
来源：http://hz.jqgfzy.top/gtseywboje.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.meibo888.top/gtludgvusq.html

[Q88] 行转列（条件聚合）
来源：http://hz.tanke756.top/gtjwmujvgr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xylfe.cn/gteaiqfzcz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yuxming.cn/gttpejrliw.html

[Q89] 判断表是否存在
来源：http://hz.yvedp.cn/gtwlciejxh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yvedp.cn/gtvlbfjshx.html

[Q90] 生成序号列
来源：http://hz.chenlongwang.top/gtccfvofil.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangtech.top/gtfyiiwrlo.html

================================================================================
来源：http://hz.xuanzx.com/gtpllstrfn.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtykarzpdj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtwmkhyjos.html

[R01] shebang 与严格模式
来源：http://hz.zhengqikj.top/gtygwoqsaw.html

#!/usr/bin/env bash
来源：http://hz.shuidangran.top/gtrgqhvihv.html

set -euo pipefail
来源：http://hz.quarkkingdee.top/gtejjrovme.html

[R02] 变量赋值与使用
来源：http://hz.bjfxy.top/gttrsutpok.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtdmridkjg.html

[R03] 只读变量
来源：http://hz.zhixingplan.top/gtjwifnkgi.html

readonly PI=3.14
来源：http://hz.zdqjudy.top/gtfzmzqktd.html

[R04] 位置参数
来源：http://hz.zhongyouzk.top/gtmlkpxnxw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fzhhl.top/gtbvctdowt.html

[R05] 参数默认值
来源：http://hz.ybcxt.top/gtjnpdslmp.html

name="${1:-default}"
来源：http://hz.zhiwuduotai.top/gtkzpulgmq.html

[R06] 判断命令是否存在
来源：http://hz.zhaomingkeji.xyz/gtnsiqeyeb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.vqdsnc.cn/gtqjtomftb.html

[R07] if 判断文件
来源：http://hz.chenzaomai.com/gtasdowvpb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yongpay.top/gtabvfnswz.html

[R08] 数值比较
来源：http://hz.daria6918.cn/gtkevnzblc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sxryk.cn/gtwskszoji.html

[R09] 字符串比较
来源：http://hz.kuanghao11.cn/gtafikzafn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhaomingkeji.xyz/gtanbvyena.html

[R10] 正则匹配
来源：http://hz.redwolf501.top/gtlykcolkf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhijiandao.cn/gtwhpohkpz.html

[R11] case 多分支
来源：http://hz.guowangkeji.top/gtcupzlzsf.html

case "$1" in
来源：http://hz.gzhubu.top/gtpnkamanj.html

start) echo "启动" ;;
来源：http://hz.dianchejie.cn/gtkjkitmcp.html

stop)  echo "停止" ;;
来源：http://hz.tianlin.xyz/gtdexuymma.html

*)     echo "未知命令" ;;
来源：http://hz.gaohongyu789.top/gtojwbwlbk.html

esac
来源：http://hz.cucudq.cn/gtvogabkye.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gtmrrpjihs.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhixingplan.top/gteujwasri.html

[R13] for 计数循环
来源：http://hz.bjfxy.top/gtifmjowkk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.316326.xyz/gthizjswjg.html

[R14] C 风格 for
来源：http://hz.ehwqpu.com/gtndgvzika.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenzaomai.com/gtxmsbqyvh.html

[R15] while 逐行读文件
来源：http://hz.c1oappe.top/gtmdpzrnhz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hysaishi.cn/gtofcyospx.html

[R16] until 等待条件
来源：http://hz.gotoacloud.top/gtuvvydgik.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangdashe.top/gtkbpuifds.html

[R17] 数组定义与取值
来源：http://hz.hnqzz.top/gtvajyithl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.9152youxi.cn/gtzrajxybr.html

[R18] 遍历数组
来源：http://hz.yuxming.cn/gtadgnndwn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.0kj1m.cn/gtnanaunxu.html

[R19] 数组长度
来源：http://hz.hywenlv.cn/gtgmucloqf.html

echo "${#arr[@]}"
来源：http://hz.chenzaomai.com/gtjgleoudp.html

[R20] 关联数组（字典）
来源：http://hz.jinqigfzy.top/gtgzzzjaom.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.0kj1m.cn/gtbxbgjidm.html

[R21] 字符串长度
来源：http://hz.haohaochexian.top/gtbnxbepui.html

echo "${#s}"
来源：http://hz.wangdashe.top/gtuqzworhg.html

[R22] 截取子串
来源：http://hz.chenzaomai.com/gtpgohfbyp.html

echo "${s:0:5}"
来源：http://hz.ydjk.org.cn/gtmtcgovax.html

[R23] 字符串替换
来源：http://hz.dashuyun.cn/gtdyhdpqgh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuetiantiany.cn/gtpaxzmxdq.html

[R24] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gtcdrnmyms.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.meibo888.top/gtdrsoytgm.html

[R25] 去后缀 / 去前缀
来源：http://hz.iojbl.cn/gtzhcjeigf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zdqjudy.top/gtctfbbgig.html

[R26] 命令替换
来源：http://hz.zhongyouzk.top/gtdkopbulp.html

now=$(date +%F); echo "$now"
来源：http://hz.52xcode.cn/gthkyvvniy.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtahnlcxyg.html

echo $((1 + 2 * 3))
来源：http://hz.iojbl.cn/gtovzpxksy.html

[R28] 浮点运算
来源：http://hz.guowangkeji.top/gtyiptzsxh.html

echo "scale=2; 10/3" | bc
来源：http://hz.bjfxy.top/gthvlyqrcl.html

[R29] 定义函数
来源：http://hz.xuetiantiany.cn/gtflvhipvn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xingfuxueyuan.xyz/gtcwwfpbsn.html

[R30] 函数返回状态码
来源：http://hz.ivvv.top/gtvkkkvmqe.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhongyouzk.top/gtufbviaxk.html

[R31] 局部变量
来源：http://hz.yonumen.top/gtvbrdodbl.html

f() { local x=1; echo "$x"; }
来源：http://hz.yuxming.cn/gtwqwuyyxq.html

[R32] 参数个数校验
来源：http://hz.yongpay.top/gtluugnnxk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gzhubu.top/gtmurlybkq.html

[R33] 捕获错误并提示行号
来源：http://hz.zhongyouzk.top/gtuabyiimo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.iojbl.cn/gtutalcpik.html

[R34] 退出时清理
来源：http://hz.316326.xyz/gtqgahopqw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jlsjyb.cn/gtlvezaxkr.html

[R35] 后台执行并等待
来源：http://hz.chenlongwang.top/gtkgfbylpv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xziqi.cn/gtmvugeavr.html

[R36] 并发执行多个任务
来源：http://hz.snrcjt.cn/gtreqdddov.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cashguo.top/gtvgkhxhmu.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gttklciuwd.html

files=$(ls -1)
来源：http://hz.yongpay.top/gtvwtyedby.html

[R38] 管道串联
来源：http://hz.fzhhl.top/gtwfrwocct.html

cat a.txt | grep -i error | wc -l
来源：http://hz.wangshuangyany.cn/gtqymexyaj.html

[R39] 重定向标准输出与错误
来源：http://hz.yonumen.top/gtomgcqjut.html

cmd > out.log 2>&1
来源：http://hz.nanxuanxn.top/gtjlcxqutc.html

[R40] 追加写日志
来源：http://hz.wangshuangyany.cn/gttvwrbzat.html

echo "log" >> out.log
来源：http://hz.nanxinkj.top/gtjtzxgtcy.html

[R41] 丢弃输出
来源：http://hz.chenjidiqi.icu/gtkkvbntjz.html

cmd >/dev/null 2>&1
来源：http://hz.sysykeji.top/gtumfosukn.html

[R42] 输入重定向
来源：http://hz.xuanzx.com/gthdwfmsxu.html

wc -l < a.txt
来源：http://hz.bjfxy.top/gthtniohww.html

[R43] 按名字查找文件
来源：http://hz.dianchejie.cn/gtkkltkixa.html

find . -name "*.log" -type f
来源：http://hz.zhiwuduotai.top/gtrfxxcpwi.html

[R44] 按修改时间查找
来源：http://hz.zdqjudy.top/gttotuspox.html

find . -mtime -7 -type f
来源：http://hz.ybcxt.top/gtfackbqja.html

[R45] 批量删除
来源：http://hz.xuanzx.com/gtsghhenqz.html

find . -name "*.tmp" -delete
来源：http://hz.c1oappe.top/gtvlvoszbz.html

[R46] 递归替换文件内容
来源：http://hz.ppjwa.cn/gtvzvtqacz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.haohaochexian.top/gtaqlvlauu.html

[R47] sed 单行替换
来源：http://hz.xingfuxueyuan.xyz/gtzitorpiy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hfpthk.cn/gtmvqyrptj.html

[R48] awk 取指定列
来源：http://hz.gogol.net.cn/gtzbifplze.html

awk '{print $1, $3}' a.txt
来源：http://hz.sysykeji.top/gtzilwzcvp.html

[R49] awk 带条件
来源：http://hz.sysykeji.top/gtmqpluydc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zycfv.cn/gtvwzzsgpc.html

[R50] awk 求和
来源：http://hz.zhaomingkeji.xyz/gtqkqvqlfr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtqqavwjcl.html

[R51] 排序去重取前几
来源：http://hz.cheryme.top/gtgfgpxqmg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yonumen.top/gttflgagxg.html

[R52] 统计行数
来源：http://hz.yj202588.top/gtyxxxzlmf.html

wc -l a.txt
来源：http://hz.yj20258.top/gtfutrvbcv.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgfzy.top/gtsjypudqo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jianghu66.top/gtvtfkeukj.html

[R54] 比较两个文件
来源：http://hz.iojbl.cn/gteqvkdoof.html

diff a.txt b.txt
来源：http://hz.zhaomingkeji.xyz/gtqypkwojw.html

[R55] 压缩与解压
来源：http://hz.shangyingyoupin.top/gtwvsjmldd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ppjwa.cn/gthiloprvj.html

[R56] 远程拷贝
来源：http://hz.aizwys.cn/gtfrsjhmpj.html

scp file user@host:/path/
来源：http://hz.zhongyouzk.top/gtlvnoitht.html

[R57] 远程执行命令
来源：http://hz.hammf.cn/gttucoanow.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtqhpclmit.html

[R58] 下载文件
来源：http://hz.cucudq.cn/gtyphmgbno.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yangfankeji.com/gtvfjigzxh.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtmfhzmxoi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydjk.org.cn/gtecpldmge.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtjzbmpljo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.dashuyun.cn/gtgqrdnzds.html

[R61] 磁盘占用
来源：http://hz.hnqzz.top/gtdfrthjpq.html

df -h;  du -sh *
来源：http://hz.gaohongyu789.top/gtsprzgftu.html

[R62] 找最占空间的文件
来源：http://hz.chenlongwang.top/gtimtkxfvm.html

du -ah . | sort -rh | head -10
来源：http://hz.iojbl.cn/gtqwkzsfcx.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gtenqhrivg.html

free -h;  ps aux | grep nginx
来源：http://hz.yvedp.cn/gtwnxacdia.html

[R64] 结束进程
来源：http://hz.hongshengwenyu.top/gtxckkpieo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xylfe.cn/gtvauuduzt.html

[R65] 查看端口占用
来源：http://hz.0kj1m.cn/gtgtmphmut.html


<!-- 参考信息 -->