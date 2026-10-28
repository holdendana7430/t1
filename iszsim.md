代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://hz.fengsongda.top/gtimwtorry.html

[Q22] 排序
来源：http://hz.zhiwuduotai.top/gtqfzrajbv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hz.sweek.top/gtyomwzczs.html

[Q23] 分页
来源：http://hz.yonumen.top/gttkycgpks.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hz.tanke756.top/gtkajscmlq.html

[Q24] 去重
来源：http://hz.xinyue.icu/gtcugbirrq.html

SELECT DISTINCT city FROM users;
来源：http://hz.jlsjyb.cn/gtpyelpazy.html

[Q25] 只取前 N 条
来源：http://hz.pycfn.com/gtaqkpxgfo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.9152youxi.cn/gtvcndghqw.html

[Q26] 计数
来源：http://hz.birdmap.top/gthvlqunna.html

SELECT COUNT(*) FROM users;
来源：http://hz.xziqi.cn/gtfihlybey.html

[Q27] 条件计数
来源：http://hz.xinyue.icu/gtzjfgioaw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.yj20258888.top/gtuafsrapl.html

[Q28] 求和与平均
来源：http://hz.316326.xyz/gtlolcmilk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.sufxvd.cn/gtdcnqolxe.html

[Q29] 最大最小值
来源：http://hz.ydzc1.top/gtupnpshtl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.xylfe.cn/gtgdoqumms.html

[Q30] 分组统计
来源：http://hz.xuanzx.com/gtvjagyuni.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.hywenlv.cn/gtfptdvgyo.html

[Q31] 分组后过滤
来源：http://hz.yj202588.top/gtgdgetrtt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.cdnleiting.top/gtlyhhftmi.html

[Q32] 分组拼接字符串
来源：http://hz.shzxlz.cn/gtgvrnnmpu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtobicgrdi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.cdnleiting.top/gtirtesapa.html

[Q33] 多列分组
来源：http://hz.haohaochexian.top/gttcwxzwnj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.shanyushiyangkeji.top/gtklwdcdzt.html

[Q34] 每组取第一条
来源：http://hz.zhengqikj.top/gtiljetbxv.html

SELECT * FROM (
来源：http://hz.ybcxt.top/gtancrvvwz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.guannengcc.top/gtajtvlvii.html

) t WHERE rn = 1;
来源：http://hz.nanxuanxn.top/gtdbrmiurz.html

[Q35] 内连接
来源：http://hz.gogol.net.cn/gtubwzndbe.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.zycfv.cn/gthiklvyei.html

[Q36] 左连接
来源：http://hz.shanyushiyangtech.top/gtfvhtfxor.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.zhongyouzk.top/gtimtizviu.html

[Q37] 右连接
来源：http://hz.daxiang520.top/gttghdcwrg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.birdmap.top/gtnjgnbyek.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.shuidangran.top/gtwrqayfip.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.yuanzhike.top/gtffvyojnh.html

[Q39] 自连接（查上下级）
来源：http://hz.316326.xyz/gtxjtzshur.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.fengsongda.top/gtxfebmiil.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.xingfuxueyuan.xyz/gtshtbqfxg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.chenzaomai.com/gtvvdcalvl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.cdnleiting.top/gtgobcdlil.html

[Q41] 多表连接
来源：http://hz.yangfankeji.com/gtltpqweih.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.shzxlz.cn/gtyelulian.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yueranfly.top/gtqqnfenkm.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.nanxinkj.top/gtbwlypzda.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangkeji.top/gtjnxzlozi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhixingplan.top/gtoaelfahz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.yangfankeji.com/gtahucfmqm.html

[Q43] 标量子查询
来源：http://hz.9152youxi.cn/gtgjevhrel.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.ywan-chungtsiang.top/gtmqgcyfih.html

[Q44] IN 子查询
来源：http://hz.xziqi.cn/gtpewmrzgf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangkeji.top/gtgmsumrcj.html

[Q45] EXISTS 判断存在
来源：http://hz.dianchejie.cn/gtcnxpzsid.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.hywenlv.cn/gtuqjbbhck.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cqqwz.cn/gtnwobnsga.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gthncnmbgf.html

[Q47] 与平均值比较
来源：http://hz.daria6918.cn/gtztpcoyex.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.chenjidiqi.icu/gtjlitjgic.html

[Q48] CTE 公用表表达式
来源：http://hz.pengpengdd.cyou/gtuorhwtno.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gtoaurzmes.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.cqqwz.cn/gtjnbcpxgm.html

[Q49] 更新单行
来源：http://hz.chenlongwang.top/gtjizzayui.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jinqigufen.top/gtrhdipkvl.html

[Q50] 批量更新
来源：http://hz.shanyushiyangtech.top/gtzaianiax.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.hysaishi.cn/gtdtqtousm.html

[Q51] 用子查询更新
来源：http://hz.xinyue.icu/gtwtnfqyqs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jqgfzy.top/gtamkvivda.html

[Q52] 删除指定行
来源：http://hz.jqgfzy.top/gtocgqhejn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.birdmap.top/gtwjfqbadb.html

[Q53] 按条件删除
来源：http://hz.nanxuanxn.top/gtvkgfxazd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.guannengcc.top/gtftxxrskx.html

[Q54] 清空表
来源：http://hz.haohaochexian.top/gtsdkawcbm.html

TRUNCATE TABLE logs;
来源：http://hz.nanxuanxn.top/gtwzessshg.html

[Q55] 排名（并列占位）
来源：http://hz.cdnleiting.top/gtzvygogba.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jinqigfzy.top/gtyyfcmxld.html

[Q56] 密集排名（并列不占位）
来源：http://hz.svipenyu.cn/gtejhbjyzi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xinyue.icu/gtqslzwyyk.html

[Q57] 行号
来源：http://hz.gzhubu.top/gtvtcpmvej.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jinyuanbaomall.cn/gtzynlaxvv.html

[Q58] 累计求和
来源：http://hz.fengsongda.top/gtalscqjfv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.316326.xyz/gtnxfgsnhu.html

[Q59] 分组内累计
来源：http://hz.sufxvd.cn/gtsftvvaif.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.iojbl.cn/gtqcdhjcvj.html

[Q60] 取上一行 / 下一行
来源：http://hz.jinyuanbaomall.cn/gtivrvfhbq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.c1oappe.top/gtuxbmqkke.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhoulong.xyz/gtqaeaxkcn.html

[Q61] 移动平均
来源：http://hz.zhiwuduotai.top/gtmnzpdiqw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.bjfxy.top/gtfownwetv.html

[Q62] 分组占比
来源：http://hz.zhengqikj.top/gteckswpsg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtpgqjsohh.html

[Q63] 开启事务
来源：http://hz.zhiwuduotai.top/gtgaeasgiu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hfpthk.cn/gtcparvxlv.html

[Q64] 提交事务
来源：http://hz.shzxlz.cn/gtbdcrecfk.html

COMMIT;
来源：http://hz.fzhhl.top/gtxcdmffjr.html

[Q65] 回滚事务
来源：http://hz.yj20258.top/gtafmcgeks.html

ROLLBACK;
来源：http://hz.havefunace.top/gttxljxjju.html

[Q66] 行锁查询
来源：http://hz.ydjk.org.cn/gtauzsdpbr.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cqqwz.cn/gttamosayz.html

[Q67] 设置隔离级别
来源：http://hz.feifeiyinyue.top/gtcidujahj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daria6918.cn/gtjgniupff.html

[Q68] 保存点
来源：http://hz.cheryme.top/gtnlczdkgy.html

SAVEPOINT sp1;
来源：http://hz.cqqwz.cn/gtjvvefblk.html

ROLLBACK TO sp1;
来源：http://hz.zhengqikj.top/gtjwidvgvg.html

[Q69] 查看执行计划
来源：http://hz.xinyue.icu/gtbeaepook.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.chenjidiqi.icu/gtffdvcabd.html

[Q70] 更新统计信息
来源：http://hz.yueranfly.top/gtwcyplijz.html

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gtdbdbryzf.html

[Q71] 查看建表语句
来源：http://hz.zhixingplan.top/gtzwarpqks.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tianlin.xyz/gthsqdgott.html

[Q72] 查看索引
来源：http://hz.nwbrower.top/gtzudaugro.html

SHOW INDEX FROM users;
来源：http://hz.ivvv.top/gtluqwsvgt.html

[Q73] 查看表状态
来源：http://hz.dianchejie.cn/gtxasbmqze.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.redwolf501.top/gtyzzfgdmi.html

[Q74] 强制使用索引
来源：http://hz.quarkkingdee.top/gtbculjchg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yj202588.top/gtzlkjkojz.html

[Q75] 日期格式化
来源：http://hz.gzhubu.top/gtqjxtgwkl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtlqkmdrpk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yonumen.top/gtkmowfzok.html

[Q76] 按天统计
来源：http://hz.zhoulong.xyz/gtdhxkmijp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dianchejie.cn/gtjpkwndvt.html

[Q77] 时间加减
来源：http://hz.nwbrower.top/gtvqvjpqfa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.0kj1m.cn/gtshrvaybu.html

[Q78] 当前时间
来源：http://hz.yuxming.cn/gtulhrnwbz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gogol.net.cn/gtonciwrtv.html

[Q79] 字符串拼接
来源：http://hz.shanyushiyangtech.top/gtepwijvxe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.chenzaomai.com/gtjgscqhmm.html

[Q80] 字符串截取
来源：http://hz.meibo888.top/gtcjybated.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenjidiqi.icu/gtvwlvnqto.html

[Q81] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtsenshdhm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxinkj.top/gtgqaccibm.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258888.top/gtytabtuwv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.haohaochexian.top/gtamdjdpxa.html

[Q83] 大小写转换
来源：http://hz.yanxiufei.cn/gtsbiiapbg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sufxvd.cn/gtorpffngy.html

[Q84] 去除首尾空格
来源：http://hz.tian-w.cn/gtkbabakvi.html

SELECT TRIM(name) FROM users;
来源：http://hz.cucudq.cn/gtcgmwbqga.html

[Q85] 数值取整
来源：http://hz.jyoumei.cn/gtctqxexnu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yueranfly.top/gtnqctpeds.html

[Q86] 读取 JSON 字段
来源：http://hz.dashuyun.cn/gterwjtnhy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.316326.xyz/gtnhdfjokl.html

[Q87] JSON 字段做条件
来源：http://hz.jlsjyb.cn/gtlvzsymwb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hywenlv.cn/gtkjainpil.html

[Q88] 行转列（条件聚合）
来源：http://hz.guannengcc.top/gtcyvaydpz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nwbrower.top/gtxniahkpr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fengsongda.top/gttukkojga.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gtejxnbdjq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.pengpengdd.cyou/gtzdlosaud.html

[Q90] 生成序号列
来源：http://hz.zhijiandao.cn/gttglhkuvr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yj20258888.top/gtbuznaugo.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtlrmookan.html

R. Bash 专题
来源：http://hz.gzhubu.top/gtrilevefa.html

================================================================================
来源：http://hz.yuanzhike.top/gtminimbbg.html

[R01] shebang 与严格模式
来源：http://hz.jinqigufen.top/gtgntxtspz.html

#!/usr/bin/env bash
来源：http://hz.yj202588.top/gtheqfndcx.html

set -euo pipefail
来源：http://hz.xingfuxueyuan.xyz/gtsdavoybo.html

[R02] 变量赋值与使用
来源：http://hz.gogol.net.cn/gtauymlalx.html

name="Tom"; echo "$name"
来源：http://hz.daria6918.cn/gtuvrlaoyu.html

[R03] 只读变量
来源：http://hz.xingfuxueyuan.xyz/gtyvfmbeuk.html

readonly PI=3.14
来源：http://hz.guowangkeji.top/gtpunwzaxa.html

[R04] 位置参数
来源：http://hz.ehwqpu.com/gtphewutyt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tianlin.xyz/gttolidzgk.html

[R05] 参数默认值
来源：http://hz.gogol.net.cn/gtjygwmpoy.html

name="${1:-default}"
来源：http://hz.zhaomingkeji.xyz/gtpzxuvvlr.html

[R06] 判断命令是否存在
来源：http://hz.zhoulong.xyz/gtococktby.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yanxiufei.cn/gtqbruaeuk.html

[R07] if 判断文件
来源：http://hz.quarkkingdee.top/gthzdlyntz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gaohongyu789.top/gtvlvczwyg.html

[R08] 数值比较
来源：http://hz.52xcode.cn/gtvmepsdqa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daria6918.cn/gtyvhuegpm.html

[R09] 字符串比较
来源：http://hz.iojbl.cn/gtcdgatuyu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jqgfzy.top/gtqlepmsub.html

[R10] 正则匹配
来源：http://hz.quarkkingdee.top/gtstxslesm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxinkj.top/gtzmrdylfb.html

[R11] case 多分支
来源：http://hz.cqqwz.cn/gtgyhfkiow.html

case "$1" in
来源：http://hz.jinqigfzy.top/gtbcvtirbt.html

start) echo "启动" ;;
来源：http://hz.ybcxt.top/gtbigeldyr.html

stop)  echo "停止" ;;
来源：http://hz.havefunace.top/gtaahvlujm.html

*)     echo "未知命令" ;;
来源：http://hz.sweek.top/gtzahmijsy.html

esac
来源：http://hz.shangyingyoupin.top/gtubafsqea.html

[R12] for 遍历文件
来源：http://hz.c1oappe.top/gtcnxhtaad.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dianchejie.cn/gtqryjfgwu.html

[R13] for 计数循环
来源：http://hz.sysykeji.top/gtjcfhdtau.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shuidangran.top/gtcwvqsklr.html

[R14] C 风格 for
来源：http://hz.yanxiufei.cn/gthbhmkpfq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258.top/gtaprfjwar.html

[R15] while 逐行读文件
来源：http://hz.yj20258888.top/gtcbntxtqr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xingfuxueyuan.xyz/gtdbccqbml.html

[R16] until 等待条件
来源：http://hz.xinyue.icu/gtlwwxhauy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zdqjudy.top/gtyjdnkrcw.html

[R17] 数组定义与取值
来源：http://hz.shanyushiyangtech.top/gtvczrvlbc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shangyingyoupin.top/gtzsjypzsr.html

[R18] 遍历数组
来源：http://hz.c1oappe.top/gtpalttjnu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xziqi.cn/gtongyhizr.html

[R19] 数组长度
来源：http://hz.gaohongyu789.top/gtocvhubrd.html

echo "${#arr[@]}"
来源：http://hz.yuanzhike.top/gthucbaxuf.html

[R20] 关联数组（字典）
来源：http://hz.gaohongyu789.top/gtfmvjspmp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.mhx1999.top/gtylcdqqkq.html

[R21] 字符串长度
来源：http://hz.jqgfzy.top/gtuyuylrvg.html

echo "${#s}"
来源：http://hz.guowangkeji.top/gtwdelrpzu.html

[R22] 截取子串
来源：http://hz.jqgufenzy.top/gtarnqvlbc.html

echo "${s:0:5}"
来源：http://hz.birdmap.top/gtosimozjz.html

[R23] 字符串替换
来源：http://hz.yuxming.cn/gtjqnkjtpm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ehwqpu.com/gtzsjiqaoi.html

[R24] 大小写转换
来源：http://hz.xinyue.icu/gtepbncdox.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fzhhl.top/gtazzusfqh.html

[R25] 去后缀 / 去前缀
来源：http://hz.ywan-chungtsiang.top/gtobbvljik.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fzhhl.top/gtjnzkkabv.html

[R26] 命令替换
来源：http://hz.xinyue.icu/gtphcextlr.html

now=$(date +%F); echo "$now"
来源：http://hz.jianghu66.top/gtwelnlwdb.html

[R27] 算术展开
来源：http://hz.ybcxt.top/gtgilczjmf.html

echo $((1 + 2 * 3))
来源：http://hz.cqqwz.cn/gtudbqlyqa.html

[R28] 浮点运算
来源：http://hz.dianchejie.cn/gtbchaoyke.html

echo "scale=2; 10/3" | bc
来源：http://hz.shanyushiyangkeji.top/gtkleyuhev.html

[R29] 定义函数
来源：http://hz.daria6918.cn/gtsasetqdq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenlongwang.top/gteqnbzkqd.html

[R30] 函数返回状态码
来源：http://hz.sysykeji.top/gtwuedjqql.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.andypj.xyz/gtecuoqqhk.html

[R31] 局部变量
来源：http://hz.daxiang520.top/gtdtdkdczx.html

f() { local x=1; echo "$x"; }
来源：http://hz.jqgfzy.top/gtdxebdgar.html

[R32] 参数个数校验
来源：http://hz.xylfe.cn/gtmdwbehgt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhongyouzk.top/gtprpfxshv.html

[R33] 捕获错误并提示行号
来源：http://hz.52xcode.cn/gtzpbpenrs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yanxiufei.cn/gtdtlxggay.html

[R34] 退出时清理
来源：http://hz.ehwqpu.com/gtqtuikljc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.snrcjt.cn/gtvpzmedhl.html

[R35] 后台执行并等待
来源：http://hz.yuanzhike.top/gtrmoxphuw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.redwolf501.top/gtqlxvqngt.html

[R36] 并发执行多个任务
来源：http://hz.yj202588.top/gtlrilpqee.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.meibo888.top/gtinwgighh.html

[R37] 把输出赋给变量
来源：http://hz.hysaishi.cn/gtsootdkub.html

files=$(ls -1)
来源：http://hz.wangshuangyany.cn/gtulhmdsxq.html

[R38] 管道串联
来源：http://hz.cdnleiting.top/gtdjkjbrok.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hnqzz.top/gtvswtvjoe.html

[R39] 重定向标准输出与错误
来源：http://hz.chenlongwang.top/gteznlmsfz.html

cmd > out.log 2>&1
来源：http://hz.aizwys.cn/gtsdyznmlj.html

[R40] 追加写日志
来源：http://hz.cucudq.cn/gtgdnwijzs.html

echo "log" >> out.log
来源：http://hz.cucudq.cn/gtgpjsqxyq.html

[R41] 丢弃输出
来源：http://hz.zdqjudy.top/gtugrrhnvb.html

cmd >/dev/null 2>&1
来源：http://hz.zdqjudy.top/gtoyqydkdu.html

[R42] 输入重定向
来源：http://hz.pengpengdd.cyou/gttcublzkv.html

wc -l < a.txt
来源：http://hz.tian-w.cn/gticdgbrop.html

[R43] 按名字查找文件
来源：http://hz.daxiang520.top/gtnzzhlkha.html

find . -name "*.log" -type f
来源：http://hz.52xcode.cn/gtpxvegpdy.html

[R44] 按修改时间查找
来源：http://hz.zhaomingkeji.xyz/gtkibybssx.html

find . -mtime -7 -type f
来源：http://hz.ydjk.org.cn/gttwfupzln.html

[R45] 批量删除
来源：http://hz.9152youxi.cn/gtraankraw.html

find . -name "*.tmp" -delete
来源：http://hz.zdqjudy.top/gtkyepvjsd.html

[R46] 递归替换文件内容
来源：http://hz.redwolf501.top/gtjfzwsczt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gaohongyu789.top/gtorhdmosx.html

[R47] sed 单行替换
来源：http://hz.daria6918.cn/gtmsrblvhh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinghuilouyu.cn/gtayfyhkoq.html

[R48] awk 取指定列
来源：http://hz.xingfuxueyuan.xyz/gtaoxrjldz.html

awk '{print $1, $3}' a.txt
来源：http://hz.bjfxy.top/gtxggufkkt.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtrkwsrbam.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cashguo.top/gtaqgfdmec.html

[R50] awk 求和
来源：http://hz.jqgufenzy.top/gtcdzzulhj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtqkawwjqq.html

[R51] 排序去重取前几
来源：http://hz.pycfn.com/gtpvcodwtp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.guannengcc.top/gtpijoqroz.html

[R52] 统计行数
来源：http://hz.meibo888.top/gtwbeqfktr.html

wc -l a.txt
来源：http://hz.ydjk.org.cn/gtkeictawl.html

[R53] 查看文件头与实时尾
来源：http://hz.yanxiufei.cn/gtmlcpwntq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yongpay.top/gtcfdflxvd.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gtrzpcnxpy.html

diff a.txt b.txt
来源：http://hz.ehwqpu.com/gtxogyrbqm.html

[R55] 压缩与解压
来源：http://hz.pycfn.com/gtvanrxycq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yvedp.cn/gtbwppwmzi.html

[R56] 远程拷贝
来源：http://hz.chenzaomai.com/gtmguumzqj.html

scp file user@host:/path/
来源：http://hz.yongpay.top/gtnjexucbh.html

[R57] 远程执行命令
来源：http://hz.cqqwz.cn/gtfmvqqomw.html

ssh user@host 'uptime'
来源：http://hz.smart0.xyz/gtissjnvcd.html

[R58] 下载文件
来源：http://hz.zhongyouzk.top/gtnqemwdue.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yvedp.cn/gtyogpedfk.html

[R59] 发 POST JSON
来源：http://hz.316326.xyz/gtmhdsscdg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gttxsklhdl.html

[R60] 只看 HTTP 状态码
来源：http://hz.yueranfly.top/gtxvxmuuhr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhaomingkeji.xyz/gtaerscpch.html

[R61] 磁盘占用
来源：http://hz.fzhhl.top/gttolvrzti.html

df -h;  du -sh *
来源：http://hz.yonumen.top/gtponeqorv.html

[R62] 找最占空间的文件
来源：http://hz.yongpay.top/gtguijmore.html

du -ah . | sort -rh | head -10
来源：http://hz.wangdashe.top/gtcliymtem.html

[R63] 内存与进程
来源：http://hz.nanxuanxn.top/gtmfuvsyas.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gthefeiqsh.html

[R64] 结束进程
来源：http://hz.fengsongda.top/gtffacwcse.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zdqjudy.top/gtdbgukcxi.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtfivhpscb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenlongwang.top/gtwtnopsez.html

[R66] 定时任务
来源：http://hz.yanxiufei.cn/gtooeacibn.html

crontab -e;  crontab -l
来源：http://hz.zhixingplan.top/gtmmjolppr.html

[R67] 生成随机十六进制串
来源：http://hz.cheryme.top/gtxcpqjtqj.html

openssl rand -hex 16
来源：http://hz.316326.xyz/gtiofhidnc.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gtrnimikyf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhaomingkeji.xyz/gtbwgstqxp.html

[R69] 生成随机密码
来源：http://hz.zhixingplan.top/gtffrqfjry.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinyuanbaomall.cn/gtivbbjnvs.html

[R70] 时间戳与互转
来源：http://hz.cashguo.top/gtrxphgluz.html

date +%s;  date -d @1700000000
来源：http://hz.hnxiangtu.top/gtrpjnwsdw.html

[R71] 日期格式化
来源：http://hz.xuetiantiany.cn/gtkxgxkizp.html


<!-- 参考信息 -->