代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.shuidangran.top/gtoxmbwllj.html

[Q24] 去重
来源：http://hz.hywenlv.cn/gtaxcigogy.html

SELECT DISTINCT city FROM users;
来源：http://hz.hfpthk.cn/gtgentliju.html

[Q25] 只取前 N 条
来源：http://hz.xylfe.cn/gtulefbmaf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.xinyue.icu/gtfryywbsb.html

[Q26] 计数
来源：http://hz.feifeiyinyue.top/gtudimqsfk.html

SELECT COUNT(*) FROM users;
来源：http://hz.zhoulong.xyz/gtzgyjnlut.html

[Q27] 条件计数
来源：http://hz.shuidangran.top/gtefezywtw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.316326.xyz/gtfcjwrvrm.html

[Q28] 求和与平均
来源：http://hz.cdnleiting.top/gtlxeubkul.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.bjfxy.top/gtjrsqflla.html

[Q29] 最大最小值
来源：http://hz.hysaishi.cn/gtlondrkfd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.ydzc1.top/gtnbnthhwz.html

[Q30] 分组统计
来源：http://hz.dianchejie.cn/gtvggobcka.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.sweek.top/gtndyldbnd.html

[Q31] 分组后过滤
来源：http://hz.0kj1m.cn/gtwjqqcpbr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.xinyue.icu/gtienytqna.html

[Q32] 分组拼接字符串
来源：http://hz.shuidangran.top/gtyfxqxtaq.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtqjvzsbzv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.c1oappe.top/gtehrrqrgk.html

[Q33] 多列分组
来源：http://hz.nanxuanxn.top/gtuleopyes.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.andypj.xyz/gterjiqyuc.html

[Q34] 每组取第一条
来源：http://hz.aibaodan.cn/gtqqaoevnv.html

SELECT * FROM (
来源：http://hz.hnxiangtu.top/gtahtlyjmw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.mhx1999.top/gtubwbirkt.html

) t WHERE rn = 1;
来源：http://hz.fzhhl.top/gtrpjshelk.html

[Q35] 内连接
来源：http://hz.dianchejie.cn/gtajxthwas.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtqxoheyzj.html

[Q36] 左连接
来源：http://hz.zhongyouzk.top/gtdydybelj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hammf.cn/gtqtgyfoys.html

[Q37] 右连接
来源：http://hz.tian-w.cn/gtuidexcok.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.gzhubu.top/gtzuycqkgp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.quarkkingdee.top/gtwzwrzbts.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.shangyingyoupin.top/gtbgdqgddl.html

[Q39] 自连接（查上下级）
来源：http://hz.hywenlv.cn/gtnesjimsz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.nanxuanxn.top/gteksbgayc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.nanxuanxn.top/gtvjarpzuw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.yongpay.top/gtuysyywia.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.iojbl.cn/gtkbjpesmd.html

[Q41] 多表连接
来源：http://hz.cdnleiting.top/gtwevbfifg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shanyushiyangtech.top/gtujlznypc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.tianlin.xyz/gttkicsafm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.cdnleiting.top/gtsjzkickv.html

[Q42] 连接条件附加过滤
来源：http://hz.jiagoushi.top/gtbdztvdxg.html

SELECT u.name, o.amount FROM users u
来源：http://hz.yj20258888.top/gtwcguwype.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shanyushiyangkeji.top/gthgdqymwz.html

[Q43] 标量子查询
来源：http://hz.yuxming.cn/gtgipyozkj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.zhiwuduotai.top/gttizfbodq.html

[Q44] IN 子查询
来源：http://hz.tianlin.xyz/gtbmdkrzer.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.svipenyu.cn/gtryjfzesf.html

[Q45] EXISTS 判断存在
来源：http://hz.ywan-chungtsiang.top/gtzvqnjbpu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ywan-chungtsiang.top/gtrbhvzats.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yongpay.top/gtftysyxur.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ybcxt.top/gtwbvkplyf.html

[Q47] 与平均值比较
来源：http://hz.chenjidiqi.icu/gtxxlrrvse.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xuetiantiany.cn/gtwivrcrjo.html

[Q48] CTE 公用表表达式
来源：http://hz.ehwqpu.com/gtogbvtiul.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zycfv.cn/gtefyuonoy.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.fzhhl.top/gtxccixehj.html

[Q49] 更新单行
来源：http://hz.xingfuxueyuan.xyz/gtsgblklcl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.hnqzz.top/gtolqfvivl.html

[Q50] 批量更新
来源：http://hz.vqdsnc.cn/gtqrufkcrb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.smart0.xyz/gtmotqkulm.html

[Q51] 用子查询更新
来源：http://hz.xuetiantiany.cn/gtuhuzyppr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nwbrower.top/gtbhovstey.html

[Q52] 删除指定行
来源：http://hz.quarkkingdee.top/gtgarrutkc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydjk.org.cn/gtiajomzbw.html

[Q53] 按条件删除
来源：http://hz.0kj1m.cn/gtqwltnwgx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhongyouzk.top/gtinsczjzl.html

[Q54] 清空表
来源：http://hz.zhixingplan.top/gtfskktkfm.html

TRUNCATE TABLE logs;
来源：http://hz.yonumen.top/gtleequfyn.html

[Q55] 排名（并列占位）
来源：http://hz.zhijiandao.cn/gtojkzhlkz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.smart0.xyz/gtbmnydenm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jinqigufen.top/gtscnjtyfj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nwbrower.top/gteyrstrxv.html

[Q57] 行号
来源：http://hz.chenjidiqi.icu/gtuvhbtlrq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guannengcc.top/gtyhxnucrt.html

[Q58] 累计求和
来源：http://hz.haohaochexian.top/gtzaplulvr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtinzdnhuq.html

[Q59] 分组内累计
来源：http://hz.daxiang520.top/gtmhcyeaau.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinqigfzy.top/gttwsduebt.html

[Q60] 取上一行 / 下一行
来源：http://hz.aizwys.cn/gteyndvzqq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhixingplan.top/gtabrsqyyo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jqgfzy.top/gtnltgboqy.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtzcxuhyqj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dianchejie.cn/gtkhfnbpbz.html

[Q62] 分组占比
来源：http://hz.shangyingyoupin.top/gtdmerdneo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jinqigfzy.top/gtvfaqfdkv.html

[Q63] 开启事务
来源：http://hz.wangshuangyany.cn/gtolwxpscw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xingfuxueyuan.xyz/gtgehthriw.html

[Q64] 提交事务
来源：http://hz.c1oappe.top/gtxwbsoozj.html

COMMIT;
来源：http://hz.yuanzhike.top/gtxxhxkmkm.html

[Q65] 回滚事务
来源：http://hz.yuanzhike.top/gtcduplytj.html

ROLLBACK;
来源：http://hz.yj202588.top/gtgzqybkvk.html

[Q66] 行锁查询
来源：http://hz.dianchejie.cn/gtlqobdoyc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenlongwang.top/gtgqpwjexf.html

[Q67] 设置隔离级别
来源：http://hz.daria6918.cn/gtvtpmcnbe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258.top/gtqqdhtyes.html

[Q68] 保存点
来源：http://hz.wangshuangyany.cn/gthxwogobb.html

SAVEPOINT sp1;
来源：http://hz.yj20258888.top/gtlboxeblp.html

ROLLBACK TO sp1;
来源：http://hz.ydzc1.top/gtixuwvjvl.html

[Q69] 查看执行计划
来源：http://hz.ybcxt.top/gthkfgrflm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj202588.top/gtqimuyege.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtvxzfokez.html

ANALYZE TABLE users;
来源：http://hz.meibo888.top/gtjevnrhec.html

[Q71] 查看建表语句
来源：http://hz.dianchejie.cn/gtzdqoptub.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ybcxt.top/gtejfurcko.html

[Q72] 查看索引
来源：http://hz.cucudq.cn/gtldqyzaxm.html

SHOW INDEX FROM users;
来源：http://hz.ybcxt.top/gtomhmpzbc.html

[Q73] 查看表状态
来源：http://hz.jinghuilouyu.cn/gtvssjszfj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.aizwys.cn/gtrsrnerur.html

[Q74] 强制使用索引
来源：http://hz.zhixingplan.top/gtalnmfack.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnxiangtu.top/gtjpttfxhl.html

[Q75] 日期格式化
来源：http://hz.sysykeji.top/gtyvjviuku.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gtnmizpbpm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxuanxn.top/gtotcjulmp.html

[Q76] 按天统计
来源：http://hz.redwolf501.top/gtvzafqyux.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtpdiqmyyg.html

[Q77] 时间加减
来源：http://hz.quarkkingdee.top/gtdewvfzpd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtdjudahnv.html

[Q78] 当前时间
来源：http://hz.redwolf501.top/gtytgwdggo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgfzy.top/gtvpbrhkco.html

[Q79] 字符串拼接
来源：http://hz.cdnleiting.top/gtqbwsmgkj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sxryk.cn/gtegvvybnt.html

[Q80] 字符串截取
来源：http://hz.feifeiyinyue.top/gtuyutynrk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cucudq.cn/gtwpbueywe.html

[Q81] 字符串替换
来源：http://hz.shuidangran.top/gtvxsjxdlt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jinyuanbaomall.cn/gtqlmugtkl.html

[Q82] 字符长度与字节长度
来源：http://hz.yonumen.top/gtgxosrgwq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.haohaochexian.top/gtpteatjxb.html

[Q83] 大小写转换
来源：http://hz.gzhubu.top/gtoafqstdn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtfinvebnt.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gtfleruzfv.html

SELECT TRIM(name) FROM users;
来源：http://hz.xylfe.cn/gtyekzmoyv.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtgkudfbkk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nwbrower.top/gtensagoht.html

[Q86] 读取 JSON 字段
来源：http://hz.jiagoushi.top/gtojrqxbkc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.meibo888.top/gtnozslzrn.html

[Q87] JSON 字段做条件
来源：http://hz.snrcjt.cn/gtjwjrdnqu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydzc1.top/gticinwabv.html

[Q88] 行转列（条件聚合）
来源：http://hz.hongshengwenyu.top/gtaigvfuvr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ivvv.top/gthhyafsvl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.snrcjt.cn/gtidphknkb.html

[Q89] 判断表是否存在
来源：http://hz.yj202588.top/gtqcuqyqkm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinghuilouyu.cn/gtcjtihehb.html

[Q90] 生成序号列
来源：http://hz.fzhhl.top/gtzuwrjowa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ybcxt.top/gtpmekneww.html

================================================================================
来源：http://hz.mhx1999.top/gtpvikqtmg.html

R. Bash 专题
来源：http://hz.xinyue.icu/gtotipipdr.html

================================================================================
来源：http://hz.nwbrower.top/gtwofaxjpf.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtevskgvgc.html

#!/usr/bin/env bash
来源：http://hz.smart0.xyz/gtvrqikfvw.html

set -euo pipefail
来源：http://hz.redwolf501.top/gtnsuqarfl.html

[R02] 变量赋值与使用
来源：http://hz.xuanzx.com/gtsroxtbsj.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtxwrmcmkn.html

[R03] 只读变量
来源：http://hz.hnxiangtu.top/gtpxpvfgnf.html

readonly PI=3.14
来源：http://hz.guowangkeji.top/gtsuxftolk.html

[R04] 位置参数
来源：http://hz.tian-w.cn/gtvhlesjlz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.c1oappe.top/gtdarhmcku.html

[R05] 参数默认值
来源：http://hz.hysaishi.cn/gtzdxvyskf.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtqocnhxsy.html

[R06] 判断命令是否存在
来源：http://hz.jiagoushi.top/gtephvpkgx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ydjk.org.cn/gtnpaeipvm.html

[R07] if 判断文件
来源：http://hz.hysaishi.cn/gtwrzgjnxw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gzhubu.top/gthzlcaxyg.html

[R08] 数值比较
来源：http://hz.chenlongwang.top/gtrbroehsg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shzxlz.cn/gtdktyhjcg.html

[R09] 字符串比较
来源：http://hz.cucudq.cn/gtncuatfvg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuetiantiany.cn/gtmrljygcg.html

[R10] 正则匹配
来源：http://hz.xingfuxueyuan.xyz/gththqeetn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtchrmdmow.html

[R11] case 多分支
来源：http://hz.zhiwuduotai.top/gtdkopjlmu.html

case "$1" in
来源：http://hz.wangdashe.top/gtzjpvdnpp.html

start) echo "启动" ;;
来源：http://hz.xinyue.icu/gtcbjgnleb.html

stop)  echo "停止" ;;
来源：http://hz.0kj1m.cn/gtfbxjhdck.html

*)     echo "未知命令" ;;
来源：http://hz.chenlongwang.top/gtpudaegck.html

esac
来源：http://hz.pycfn.com/gtuurkfyyt.html

[R12] for 遍历文件
来源：http://hz.snrcjt.cn/gtlhfwoufh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gzhubu.top/gtxyhrgmkt.html

[R13] for 计数循环
来源：http://hz.xinyue.icu/gtdqowaggt.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cucudq.cn/gtqfwtfyfh.html

[R14] C 风格 for
来源：http://hz.shanyushiyangkeji.top/gtehwvcslk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cashguo.top/gtvtomtyps.html

[R15] while 逐行读文件
来源：http://hz.gaohongyu789.top/gtvsgaivua.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.0kj1m.cn/gtrablbzih.html

[R16] until 等待条件
来源：http://hz.fengsongda.top/gtftzktdlg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.guannengcc.top/gtscihimav.html

[R17] 数组定义与取值
来源：http://hz.sxryk.cn/gtvbndxxah.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.redwolf501.top/gtqviuywcl.html

[R18] 遍历数组
来源：http://hz.yanxiufei.cn/gtwgiinzna.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ywan-chungtsiang.top/gtwzmgbvvq.html

[R19] 数组长度
来源：http://hz.wangdashe.top/gtqivaaypm.html

echo "${#arr[@]}"
来源：http://hz.jinyuanbaomall.cn/gtufskqwvw.html

[R20] 关联数组（字典）
来源：http://hz.zhoulong.xyz/gtrmvgbctf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhiwuduotai.top/gtuhdrlapy.html

[R21] 字符串长度
来源：http://hz.dianchejie.cn/gtmkycneqr.html

echo "${#s}"
来源：http://hz.hnqzz.top/gtzxwtxgyh.html

[R22] 截取子串
来源：http://hz.chenzaomai.com/gtlqrzofgf.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gtrjpjuzkk.html

[R23] 字符串替换
来源：http://hz.shzxlz.cn/gticuhsbck.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.mhx1999.top/gtsvkqvykm.html

[R24] 大小写转换
来源：http://hz.pycfn.com/gtmkflvidz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yanxiufei.cn/gtqrlgzots.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgufenzy.top/gtvbntoqsh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.smart0.xyz/gtoxjcdbxt.html

[R26] 命令替换
来源：http://hz.birdmap.top/gtelidsejv.html

now=$(date +%F); echo "$now"
来源：http://hz.ivvv.top/gttwdheqen.html

[R27] 算术展开
来源：http://hz.shzxlz.cn/gtlfmfdifk.html

echo $((1 + 2 * 3))
来源：http://hz.hnxiangtu.top/gtulnadigu.html

[R28] 浮点运算
来源：http://hz.cdnleiting.top/gtcjwrtzlp.html

echo "scale=2; 10/3" | bc
来源：http://hz.pengpengdd.cyou/gtvajvbrfs.html

[R29] 定义函数
来源：http://hz.yonumen.top/gtcityzkej.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinghuilouyu.cn/gtywbbfbxp.html

[R30] 函数返回状态码
来源：http://hz.jinqigfzy.top/gtszxhsljm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gtlbvxzuyb.html

[R31] 局部变量
来源：http://hz.yj20258888.top/gtvtlhkrpo.html

f() { local x=1; echo "$x"; }
来源：http://hz.fengsongda.top/gtqeunyjeu.html

[R32] 参数个数校验
来源：http://hz.fzhhl.top/gtxhktbzas.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gaohongyu789.top/gtzscamkln.html

[R33] 捕获错误并提示行号
来源：http://hz.havefunace.top/gtacqgytkh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xingfuxueyuan.xyz/gtvprufixm.html

[R34] 退出时清理
来源：http://hz.birdmap.top/gtaylzrijp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtkyeqrilt.html

[R35] 后台执行并等待
来源：http://hz.tanke756.top/gtdmqaxelf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gzhubu.top/gtmhzoctux.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtmflgdzrb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangkeji.top/gttanuqdyg.html

[R37] 把输出赋给变量
来源：http://hz.cashguo.top/gtyqoisklw.html

files=$(ls -1)
来源：http://hz.yvedp.cn/gtvhtskkrj.html

[R38] 管道串联
来源：http://hz.nanxuanxn.top/gtrjxlhyoi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.snrcjt.cn/gtecqksrif.html

[R39] 重定向标准输出与错误
来源：http://hz.ybcxt.top/gtycsaahka.html

cmd > out.log 2>&1
来源：http://hz.zhoulong.xyz/gtsuhahwtg.html

[R40] 追加写日志
来源：http://hz.sufxvd.cn/gtpqyzdjvk.html

echo "log" >> out.log
来源：http://hz.quarkkingdee.top/gtohhlhtsq.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtyhsxqgmf.html

cmd >/dev/null 2>&1
来源：http://hz.chenlongwang.top/gtixgtzipt.html

[R42] 输入重定向
来源：http://hz.gogol.net.cn/gtmjugnqeo.html

wc -l < a.txt
来源：http://hz.cdnleiting.top/gthhleluii.html

[R43] 按名字查找文件
来源：http://hz.iojbl.cn/gtpulspozo.html

find . -name "*.log" -type f
来源：http://hz.cqqwz.cn/gthldxzdul.html

[R44] 按修改时间查找
来源：http://hz.fzhhl.top/gtiwcwpsfv.html

find . -mtime -7 -type f
来源：http://hz.jqgufenzy.top/gtvpdnjpvf.html

[R45] 批量删除
来源：http://hz.xziqi.cn/gtnkxwyyma.html

find . -name "*.tmp" -delete
来源：http://hz.quarkkingdee.top/gtnaevrwqr.html

[R46] 递归替换文件内容
来源：http://hz.yanxiufei.cn/gtorlsjygk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.andypj.xyz/gtojwwusdx.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtwsmnxmzo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258.top/gtjulglaxp.html

[R48] awk 取指定列
来源：http://hz.cashguo.top/gtxoygxpjb.html

awk '{print $1, $3}' a.txt
来源：http://hz.guowangkeji.top/gtsomnlqwt.html

[R49] awk 带条件
来源：http://hz.andypj.xyz/gtudfvrmaf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj202588.top/gtaloynlhr.html

[R50] awk 求和
来源：http://hz.pycfn.com/gteslzupux.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yonumen.top/gtnicbtazp.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gtshrdisfs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhoulong.xyz/gtpznocfxf.html

[R52] 统计行数
来源：http://hz.bjfxy.top/gtbtqkenaz.html

wc -l a.txt
来源：http://hz.yj20258.top/gtkebskoyt.html

[R53] 查看文件头与实时尾
来源：http://hz.zhaomingkeji.xyz/gteqmfuofa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gotoacloud.top/gtcxszlvux.html

[R54] 比较两个文件
来源：http://hz.sweek.top/gtezeaqrqv.html

diff a.txt b.txt
来源：http://hz.chenjidiqi.icu/gtwntvmhoq.html

[R55] 压缩与解压
来源：http://hz.aibaodan.cn/gtiazixrxe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shangyingyoupin.top/gtnntbhmef.html

[R56] 远程拷贝
来源：http://hz.zhixingplan.top/gtkdmlwegl.html

scp file user@host:/path/
来源：http://hz.cucudq.cn/gtobwpwavv.html

[R57] 远程执行命令
来源：http://hz.zdqjudy.top/gtpqydyasu.html

ssh user@host 'uptime'
来源：http://hz.sxryk.cn/gtepfliaoc.html

[R58] 下载文件
来源：http://hz.hammf.cn/gtvisuspel.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xylfe.cn/gtvyuxpvxr.html

[R59] 发 POST JSON
来源：http://hz.gotoacloud.top/gtukowsynt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xylfe.cn/gtvlfxtcyp.html

[R60] 只看 HTTP 状态码
来源：http://hz.yanxiufei.cn/gtihxjylfc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ppjwa.cn/gtfxtpwivo.html

[R61] 磁盘占用
来源：http://hz.ehwqpu.com/gtrjzxzovj.html

df -h;  du -sh *
来源：http://hz.bjfxy.top/gtztdabjfn.html

[R62] 找最占空间的文件
来源：http://hz.xinyue.icu/gtrrhoabvh.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtuguyxohs.html

[R63] 内存与进程
来源：http://hz.yvedp.cn/gtgvorfvkz.html

free -h;  ps aux | grep nginx
来源：http://hz.sxryk.cn/gtdzqlpfie.html

[R64] 结束进程
来源：http://hz.kuanghao11.cn/gtewshdvhd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangkeji.top/gtswriwawb.html

[R65] 查看端口占用
来源：http://hz.xziqi.cn/gtvbkamwit.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.dianchejie.cn/gtpdgqyxma.html

[R66] 定时任务
来源：http://hz.c1oappe.top/gtxphtspbn.html

crontab -e;  crontab -l
来源：http://hz.hongshengwenyu.top/gthraubfix.html

[R67] 生成随机十六进制串
来源：http://hz.jianghu66.top/gtlevtptta.html

openssl rand -hex 16
来源：http://hz.tian-w.cn/gtrljavlih.html

[R68] 计算文件校验值
来源：http://hz.fzhhl.top/gtynvtmpaa.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtahetljbp.html

[R69] 生成随机密码
来源：http://hz.hammf.cn/gtlbkfxhlp.html

head -c 16 /dev/urandom | base64
来源：http://hz.cqqwz.cn/gtjugletlj.html

[R70] 时间戳与互转
来源：http://hz.xinyue.icu/gthainldrz.html

date +%s;  date -d @1700000000
来源：http://hz.svipenyu.cn/gtraqajgfy.html

[R71] 日期格式化
来源：http://hz.yanxiufei.cn/gtcwiqzsqh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tianlin.xyz/gtihrbigkm.html

[R72] 等待端口就绪
来源：http://hz.guannengcc.top/gtzyliilpo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gtclmtymfh.html

[R73] 分割大日志
来源：http://hz.iojbl.cn/gtbrnxupvr.html


<!-- 参考信息 -->