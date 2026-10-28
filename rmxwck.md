代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.ybcxt.top/gtoukvaotb.html

[Q22] 排序
来源：http://hz.shanyushiyangkeji.top/gtgwhbwfuz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.gzhubu.top/gtxquexfpm.html

[Q23] 分页
来源：http://hz.jinqigfzy.top/gtvgogykfn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.daxiang520.top/gtfcpgeols.html

[Q24] 去重
来源：http://hz.9152youxi.cn/gtzqyybsws.html

SELECT DISTINCT city FROM users;
来源：http://hz.kuanghao11.cn/gtallxxefb.html

[Q25] 只取前 N 条
来源：http://hz.yangfankeji.com/gttimuwiqb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.yvedp.cn/gtjqurudex.html

[Q26] 计数
来源：http://hz.bjfxy.top/gtvusnqmlq.html

SELECT COUNT(*) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtccvdgpqe.html

[Q27] 条件计数
来源：http://hz.gogol.net.cn/gttfeqsoos.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.jqgfzy.top/gtiqfwyitm.html

[Q28] 求和与平均
来源：http://hz.52xcode.cn/gtzgenkdqq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.jlsjyb.cn/gtvqxdfdnu.html

[Q29] 最大最小值
来源：http://hz.xingfuxueyuan.xyz/gtcuwdmusw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.yuxming.cn/gtsngsyuax.html

[Q30] 分组统计
来源：http://hz.xuetiantiany.cn/gtyssuypsh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gttiirqbzl.html

[Q31] 分组后过滤
来源：http://hz.jianghu66.top/gtelabnebp.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.0kj1m.cn/gtzrwfnlox.html

[Q32] 分组拼接字符串
来源：http://hz.yonumen.top/gtnolyazcm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtlwzivacv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.snrcjt.cn/gtepzjcsjg.html

[Q33] 多列分组
来源：http://hz.mhx1999.top/gtfswktajt.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.jiagoushi.top/gtpfvpflem.html

[Q34] 每组取第一条
来源：http://hz.guowangkeji.top/gttolgpvru.html

SELECT * FROM (
来源：http://hz.yueranfly.top/gtzrmnseyp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.jqgufenzy.top/gtxxfdudlg.html

) t WHERE rn = 1;
来源：http://hz.pycfn.com/gtdybzzlua.html

[Q35] 内连接
来源：http://hz.daria6918.cn/gtbftfnwma.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.yanxiufei.cn/gtltxxghqr.html

[Q36] 左连接
来源：http://hz.jiagoushi.top/gterfltjjq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.hywenlv.cn/gtrjjrfoyg.html

[Q37] 右连接
来源：http://hz.hywenlv.cn/gttevlxpyd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.dianchejie.cn/gtppmebqyg.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.daria6918.cn/gtkridkswn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.hnxiangtu.top/gteauowoge.html

[Q39] 自连接（查上下级）
来源：http://hz.jinyuanbaomall.cn/gtjnypbguo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.tianlin.xyz/gtvqlycqug.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ivvv.top/gtzbykgbni.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.ybcxt.top/gtqkbueopo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.daxiang520.top/gtxzkhuevy.html

[Q41] 多表连接
来源：http://hz.ppjwa.cn/gtpqzzgjey.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.smart0.xyz/gtlnwsgnwn.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinqigufen.top/gtbkxalogf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.52xcode.cn/gtikaxlxyr.html

[Q42] 连接条件附加过滤
来源：http://hz.0kj1m.cn/gtyskzqwzy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hfpthk.cn/gtdnzmhitc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxuanxn.top/gtgrxlxhgq.html

[Q43] 标量子查询
来源：http://hz.yvedp.cn/gtxpeuqjtj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xylfe.cn/gtljwjydzn.html

[Q44] IN 子查询
来源：http://hz.zhixingplan.top/gtrnyjajuj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.ivvv.top/gtsotaqusq.html

[Q45] EXISTS 判断存在
来源：http://hz.316326.xyz/gthlxoocdr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhixingplan.top/gtltjrnsjt.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ppjwa.cn/gtswrtiyhw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.haohaochexian.top/gtnmysheou.html

[Q47] 与平均值比较
来源：http://hz.xylfe.cn/gtvpnwowzl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gaohongyu789.top/gtjphwlopt.html

[Q48] CTE 公用表表达式
来源：http://hz.xinyue.icu/gtremzljsj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jiagoushi.top/gtnxdnlfoq.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.xingfuxueyuan.xyz/gtbgddovkf.html

[Q49] 更新单行
来源：http://hz.andypj.xyz/gtkyqrvore.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinyuanbaomall.cn/gtrrwifmvt.html

[Q50] 批量更新
来源：http://hz.jiagoushi.top/gtzcufroyg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.svipenyu.cn/gtlrclmqbo.html

[Q51] 用子查询更新
来源：http://hz.jinqigufen.top/gtiygxlroi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.redwolf501.top/gtgrkcceet.html

[Q52] 删除指定行
来源：http://hz.zhoulong.xyz/gtbwvytwyo.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gtaswzyevk.html

[Q53] 按条件删除
来源：http://hz.yvedp.cn/gtfdorrhrc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.iojbl.cn/gtmlobrupb.html

[Q54] 清空表
来源：http://hz.xinyue.icu/gtowvzqbyt.html

TRUNCATE TABLE logs;
来源：http://hz.zhoulong.xyz/gtsnjvyefy.html

[Q55] 排名（并列占位）
来源：http://hz.hywenlv.cn/gthwtffrlw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.c1oappe.top/gtrbadattn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gaohongyu789.top/gtkjholgml.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gttgzlxvup.html

[Q57] 行号
来源：http://hz.xinyue.icu/gthnzbimdg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hnqzz.top/gtgggmfppq.html

[Q58] 累计求和
来源：http://hz.smart0.xyz/gtaqeboyay.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.zdqjudy.top/gtxultlnxl.html

[Q59] 分组内累计
来源：http://hz.sxryk.cn/gtwdgtbzfz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hnqzz.top/gtfsmghsys.html

[Q60] 取上一行 / 下一行
来源：http://hz.yonumen.top/gtaltfdpai.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tian-w.cn/gtkpeqftoh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhijiandao.cn/gtihlyrmrb.html

[Q61] 移动平均
来源：http://hz.hammf.cn/gtebqtcnuo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xinyue.icu/gtratbrejv.html

[Q62] 分组占比
来源：http://hz.yueranfly.top/gtspfwgnro.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtdyneduoq.html

[Q63] 开启事务
来源：http://hz.zhiwuduotai.top/gtdfbvygkt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zdqjudy.top/gtsfizmbwm.html

[Q64] 提交事务
来源：http://hz.gogol.net.cn/gtuywrmqrz.html

COMMIT;
来源：http://hz.snrcjt.cn/gtjgeyohsw.html

[Q65] 回滚事务
来源：http://hz.zhoulong.xyz/gtuzzmjvhp.html

ROLLBACK;
来源：http://hz.hongshengwenyu.top/gtvylsrewi.html

[Q66] 行锁查询
来源：http://hz.sysykeji.top/gtxbifvuco.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.52xcode.cn/gthfyinbcr.html

[Q67] 设置隔离级别
来源：http://hz.redwolf501.top/gtqiveeelm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yanxiufei.cn/gtcrtjjlzu.html

[Q68] 保存点
来源：http://hz.chenlongwang.top/gtudkfafym.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtrvrvpjvl.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangkeji.top/gttxylzjko.html

[Q69] 查看执行计划
来源：http://hz.chenjidiqi.icu/gtgwuckulc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhengqikj.top/gtqyvupoec.html

[Q70] 更新统计信息
来源：http://hz.chenlongwang.top/gtxitjmgje.html

ANALYZE TABLE users;
来源：http://hz.yj20258888.top/gtypwudwxo.html

[Q71] 查看建表语句
来源：http://hz.xylfe.cn/gtdpoykrdr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuanzx.com/gtnxynluzk.html

[Q72] 查看索引
来源：http://hz.pycfn.com/gtxzsntahv.html

SHOW INDEX FROM users;
来源：http://hz.xinyue.icu/gtnaittlha.html

[Q73] 查看表状态
来源：http://hz.fzhhl.top/gtjkxitcky.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ydjk.org.cn/gtffsscoct.html

[Q74] 强制使用索引
来源：http://hz.mhx1999.top/gtjoxzjzxe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.aizwys.cn/gtovxxynvp.html

[Q75] 日期格式化
来源：http://hz.meibo888.top/gtfcpmfoen.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.snrcjt.cn/gtinywuzwm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zycfv.cn/gtcrcifebl.html

[Q76] 按天统计
来源：http://hz.9152youxi.cn/gtczpbpvli.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dianchejie.cn/gtirigbikc.html

[Q77] 时间加减
来源：http://hz.xinyue.icu/gtswylekox.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258.top/gtrahwhjax.html

[Q78] 当前时间
来源：http://hz.feifeiyinyue.top/gtckrlggpw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shanyushiyangtech.top/gtdomogqfc.html

[Q79] 字符串拼接
来源：http://hz.0kj1m.cn/gtfxkhrlni.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shuidangran.top/gtprwkjwix.html

[Q80] 字符串截取
来源：http://hz.hnxiangtu.top/gtpyavyxtc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtxxnyyagn.html

[Q81] 字符串替换
来源：http://hz.shuidangran.top/gtiwuzaadi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tianlin.xyz/gtqodbetda.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gttvuwgicm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.quarkkingdee.top/gtnrhglsvf.html

[Q83] 大小写转换
来源：http://hz.aibaodan.cn/gtcjvnitqy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgfzy.top/gtswevragy.html

[Q84] 去除首尾空格
来源：http://hz.havefunace.top/gtuciinrjx.html

SELECT TRIM(name) FROM users;
来源：http://hz.aibaodan.cn/gtajbolupl.html

[Q85] 数值取整
来源：http://hz.chenjidiqi.icu/gtqkfgpdrl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xuetiantiany.cn/gtrsrnmdqb.html

[Q86] 读取 JSON 字段
来源：http://hz.hysaishi.cn/gtulqdytnn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.havefunace.top/gtwllfbmsm.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtihmqaigp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhengqikj.top/gtwxhivhvd.html

[Q88] 行转列（条件聚合）
来源：http://hz.xziqi.cn/gtgqeravmy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.guannengcc.top/gtqxezqfcd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtbzghouvv.html

[Q89] 判断表是否存在
来源：http://hz.birdmap.top/gtwbikqnyj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cdnleiting.top/gtkxshthyt.html

[Q90] 生成序号列
来源：http://hz.ppjwa.cn/gtfdxsldxc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.nwbrower.top/gtbswnihtj.html

================================================================================
来源：http://hz.c1oappe.top/gtbhbmdxsb.html

R. Bash 专题
来源：http://hz.jyoumei.cn/gtqgystzce.html

================================================================================
来源：http://hz.cashguo.top/gtglopybew.html

[R01] shebang 与严格模式
来源：http://hz.cheryme.top/gtutnlcfjn.html

#!/usr/bin/env bash
来源：http://hz.cqqwz.cn/gtzaklfbgm.html

set -euo pipefail
来源：http://hz.zhiwuduotai.top/gtrjtgqzuh.html

[R02] 变量赋值与使用
来源：http://hz.jinyuanbaomall.cn/gtzwqmrgwo.html

name="Tom"; echo "$name"
来源：http://hz.sxryk.cn/gtgjfrdepl.html

[R03] 只读变量
来源：http://hz.dianchejie.cn/gtwgxkbonp.html

readonly PI=3.14
来源：http://hz.daria6918.cn/gtrnvrxhtx.html

[R04] 位置参数
来源：http://hz.smart0.xyz/gtqrqgixbz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ybcxt.top/gtzkytcdhl.html

[R05] 参数默认值
来源：http://hz.quarkkingdee.top/gtgwzscpyu.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtopbrcqrm.html

[R06] 判断命令是否存在
来源：http://hz.ehwqpu.com/gtfgwoajwl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ppjwa.cn/gtpateykiz.html

[R07] if 判断文件
来源：http://hz.birdmap.top/gthgbsjkge.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.birdmap.top/gtkxbnfzlr.html

[R08] 数值比较
来源：http://hz.gogol.net.cn/gtxsqxeqxb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xingfuxueyuan.xyz/gtwgugpfwb.html

[R09] 字符串比较
来源：http://hz.shangyingyoupin.top/gtfbjtydqg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zdqjudy.top/gtnpsphdxv.html

[R10] 正则匹配
来源：http://hz.zhongyouzk.top/gtusnnagkg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigufen.top/gtinyaatsf.html

[R11] case 多分支
来源：http://hz.yonumen.top/gtqzkgacia.html

case "$1" in
来源：http://hz.zhengqikj.top/gtuvijtqjx.html

start) echo "启动" ;;
来源：http://hz.hnxiangtu.top/gtqmwcchbq.html

stop)  echo "停止" ;;
来源：http://hz.xuetiantiany.cn/gtszkcnyqp.html

*)     echo "未知命令" ;;
来源：http://hz.yongpay.top/gthuljnipi.html

esac
来源：http://hz.ywan-chungtsiang.top/gtrbrjyflj.html

[R12] for 遍历文件
来源：http://hz.yanxiufei.cn/gtwuoiroeu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tian-w.cn/gtcdmywwat.html

[R13] for 计数循环
来源：http://hz.zhiwuduotai.top/gthardvghm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtarihedrw.html

[R14] C 风格 for
来源：http://hz.haohaochexian.top/gtythkeacm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shuidangran.top/gtipuvsuul.html

[R15] while 逐行读文件
来源：http://hz.c1oappe.top/gtoemxjciq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.iojbl.cn/gtuuuayvax.html

[R16] until 等待条件
来源：http://hz.cheryme.top/gtnlxvzvuc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.c1oappe.top/gtukbdxvfe.html

[R17] 数组定义与取值
来源：http://hz.zhixingplan.top/gtiltjtjus.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangshuangyany.cn/gtiorwowit.html

[R18] 遍历数组
来源：http://hz.snrcjt.cn/gtvohockuj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hammf.cn/gtwoddpanl.html

[R19] 数组长度
来源：http://hz.tian-w.cn/gtuwfjphtn.html

echo "${#arr[@]}"
来源：http://hz.wangdashe.top/gtwabbpndx.html

[R20] 关联数组（字典）
来源：http://hz.ydzc1.top/gthzngdgly.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hywenlv.cn/gthoolgbzj.html

[R21] 字符串长度
来源：http://hz.9152youxi.cn/gtgncutfeb.html

echo "${#s}"
来源：http://hz.pycfn.com/gtlokmnhxg.html

[R22] 截取子串
来源：http://hz.yongpay.top/gtjjgptivo.html

echo "${s:0:5}"
来源：http://hz.xuanzx.com/gtpxrjawdh.html

[R23] 字符串替换
来源：http://hz.zhoulong.xyz/gtzmajxdzu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xziqi.cn/gtqurziast.html

[R24] 大小写转换
来源：http://hz.yuxming.cn/gtnisggtzw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhiwuduotai.top/gtqezjamwa.html

[R25] 去后缀 / 去前缀
来源：http://hz.dianchejie.cn/gtqlnmjhdo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenlongwang.top/gtlsebbdob.html

[R26] 命令替换
来源：http://hz.yj20258888.top/gtajaqodpk.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxinkj.top/gtwiugrobs.html

[R27] 算术展开
来源：http://hz.ppjwa.cn/gtflsxolpx.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gtinhwcylj.html

[R28] 浮点运算
来源：http://hz.ppjwa.cn/gtaknjhksw.html

echo "scale=2; 10/3" | bc
来源：http://hz.redwolf501.top/gtkdpeqkhw.html

[R29] 定义函数
来源：http://hz.vqdsnc.cn/gtzwjfruzn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tianlin.xyz/gtvgygwgtp.html

[R30] 函数返回状态码
来源：http://hz.hammf.cn/gtjtpextpk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.dashuyun.cn/gtlphtrspj.html

[R31] 局部变量
来源：http://hz.0kj1m.cn/gtkoifliwy.html

f() { local x=1; echo "$x"; }
来源：http://hz.tian-w.cn/gtzqbdmpxu.html

[R32] 参数个数校验
来源：http://hz.ivvv.top/gtapyoejuf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.c1oappe.top/gtpsrcltyr.html

[R33] 捕获错误并提示行号
来源：http://hz.tianlin.xyz/gtacjczrwi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daxiang520.top/gtsnnfzrem.html

[R34] 退出时清理
来源：http://hz.quarkkingdee.top/gtparlshfi.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gthenmevjc.html

[R35] 后台执行并等待
来源：http://hz.hnxiangtu.top/gtkqqqwxqu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pycfn.com/gttqrboqwc.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtlpfrzdla.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dashuyun.cn/gtaerjpyqy.html

[R37] 把输出赋给变量
来源：http://hz.jinqigufen.top/gtogimgmqn.html

files=$(ls -1)
来源：http://hz.xingfuxueyuan.xyz/gtvfvnfbxr.html

[R38] 管道串联
来源：http://hz.yuxming.cn/gtibhkzcgy.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yongpay.top/gtrbdgcdyh.html

[R39] 重定向标准输出与错误
来源：http://hz.ehwqpu.com/gtupxneoes.html

cmd > out.log 2>&1
来源：http://hz.wangdashe.top/gtyewsplci.html

[R40] 追加写日志
来源：http://hz.haohaochexian.top/gthczqgnvb.html

echo "log" >> out.log
来源：http://hz.hfpthk.cn/gtuiasmlyy.html

[R41] 丢弃输出
来源：http://hz.nwbrower.top/gtsochdqdh.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gtjjkgimsm.html

[R42] 输入重定向
来源：http://hz.xylfe.cn/gttlabpjjz.html

wc -l < a.txt
来源：http://hz.zhengqikj.top/gtbhlfzzbo.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtnbmlmvfw.html

find . -name "*.log" -type f
来源：http://hz.jinyuanbaomall.cn/gtqlfbjzrk.html

[R44] 按修改时间查找
来源：http://hz.redwolf501.top/gtguesjxnk.html

find . -mtime -7 -type f
来源：http://hz.hysaishi.cn/gtekdjlgot.html

[R45] 批量删除
来源：http://hz.sufxvd.cn/gtocppszkk.html

find . -name "*.tmp" -delete
来源：http://hz.smart0.xyz/gtjeasgyrt.html

[R46] 递归替换文件内容
来源：http://hz.hfpthk.cn/gtnlvnzhvc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.c1oappe.top/gtmznidrxx.html

[R47] sed 单行替换
来源：http://hz.hysaishi.cn/gtzertgyua.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hywenlv.cn/gtwunlphis.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtkuuyevur.html

awk '{print $1, $3}' a.txt
来源：http://hz.0kj1m.cn/gtrjzspjhq.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtxpywtqyr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cheryme.top/gtnzqeafmm.html

[R50] awk 求和
来源：http://hz.ivvv.top/gtqdjpmbhv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xylfe.cn/gtcyjkvzyz.html

[R51] 排序去重取前几
来源：http://hz.hfpthk.cn/gtiahatewm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cqqwz.cn/gtmkljeeap.html

[R52] 统计行数
来源：http://hz.yuanzhike.top/gtggbpjhro.html

wc -l a.txt
来源：http://hz.zhengqikj.top/gtarlhtpgb.html

[R53] 查看文件头与实时尾
来源：http://hz.redwolf501.top/gtcqgcqpdz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sxryk.cn/gtgynmvcki.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtanmskoaj.html

diff a.txt b.txt
来源：http://hz.xingfuxueyuan.xyz/gtevyhfvrp.html

[R55] 压缩与解压
来源：http://hz.ydjk.org.cn/gtkzailclw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hywenlv.cn/gtzcajdzkj.html

[R56] 远程拷贝
来源：http://hz.sxryk.cn/gtssegkjey.html

scp file user@host:/path/
来源：http://hz.316326.xyz/gthgbrtqwv.html

[R57] 远程执行命令
来源：http://hz.kuanghao11.cn/gtavtejvvu.html

ssh user@host 'uptime'
来源：http://hz.xuetiantiany.cn/gtxfvehsnf.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtmxatrwee.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj20258.top/gtdyekfius.html

[R59] 发 POST JSON
来源：http://hz.ydzc1.top/gtrzcutvgg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangkeji.top/gtnpmdaxgw.html

[R60] 只看 HTTP 状态码
来源：http://hz.gogol.net.cn/gtgvkddesj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ivvv.top/gtibremlte.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gtukshwltk.html

df -h;  du -sh *
来源：http://hz.cqqwz.cn/gtmwdzldmt.html

[R62] 找最占空间的文件
来源：http://hz.dianchejie.cn/gtdrqiwipn.html

du -ah . | sort -rh | head -10
来源：http://hz.pengpengdd.cyou/gtxzzwmidh.html

[R63] 内存与进程
来源：http://hz.shuidangran.top/gtozkdeacw.html

free -h;  ps aux | grep nginx
来源：http://hz.hnqzz.top/gtfhdjnejx.html

[R64] 结束进程
来源：http://hz.jqgfzy.top/gtkxklgdkj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.dianchejie.cn/gtjnnxzvmr.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtrfujsmwd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shuidangran.top/gtsyvtxdzq.html

[R66] 定时任务
来源：http://hz.cashguo.top/gtqksdkrnm.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtzunqvglg.html

[R67] 生成随机十六进制串
来源：http://hz.9152youxi.cn/gtlrsqesbe.html

openssl rand -hex 16
来源：http://hz.zhoulong.xyz/gtkaxydgan.html

[R68] 计算文件校验值
来源：http://hz.chenzaomai.com/gtcurxrpcd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhengqikj.top/gtnwmrgtcd.html

[R69] 生成随机密码
来源：http://hz.zhiwuduotai.top/gtuedttcjv.html

head -c 16 /dev/urandom | base64
来源：http://hz.havefunace.top/gtrvtdaccb.html

[R70] 时间戳与互转
来源：http://hz.zycfv.cn/gtpckdrgvk.html

date +%s;  date -d @1700000000
来源：http://hz.mhx1999.top/gtfueoofvo.html

[R71] 日期格式化
来源：http://hz.aizwys.cn/gtncfrrfon.html


<!-- 参考信息 -->