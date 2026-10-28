代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.birdmap.top/gtylegprag.html

[Q28] 求和与平均
来源：http://hz.yuxming.cn/gtmmdvdfzb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.iojbl.cn/gtgtfdgrpi.html

[Q29] 最大最小值
来源：http://hz.sweek.top/gtwobkbvol.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.shzxlz.cn/gtnhmyffcr.html

[Q30] 分组统计
来源：http://hz.yangfankeji.com/gthbxyflmz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.cashguo.top/gtxajsgzuo.html

[Q31] 分组后过滤
来源：http://hz.hongshengwenyu.top/gthcaboyyt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.yonumen.top/gtkihltgbf.html

[Q32] 分组拼接字符串
来源：http://hz.smart0.xyz/gtyamlsqgf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.sxryk.cn/gtdkfabyef.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.yvedp.cn/gtuadzmwsf.html

[Q33] 多列分组
来源：http://hz.ybcxt.top/gtyacuefzm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.ivvv.top/gtofznzzlr.html

[Q34] 每组取第一条
来源：http://hz.dashuyun.cn/gtrorzbwhm.html

SELECT * FROM (
来源：http://hz.jqgufenzy.top/gtflncynlx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.yj20258.top/gtavljjhmc.html

) t WHERE rn = 1;
来源：http://hz.smart0.xyz/gtyaypekhx.html

[Q35] 内连接
来源：http://hz.yanxiufei.cn/gtuushbffu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.smart0.xyz/gtpdwrkwds.html

[Q36] 左连接
来源：http://hz.yj20258888.top/gtojhiskac.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenzaomai.com/gthoqzlnvq.html

[Q37] 右连接
来源：http://hz.nanxinkj.top/gtudxsqkkr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.nanxuanxn.top/gthhbfzhmc.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.nanxinkj.top/gtxwekzrcv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.svipenyu.cn/gtjkyfhxcz.html

[Q39] 自连接（查上下级）
来源：http://hz.jianghu66.top/gtkkvyuwyn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yangfankeji.com/gteqsstezx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yongpay.top/gtjdjwgpyk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.sufxvd.cn/gttmwaljsi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.fengsongda.top/gtkoorsdwf.html

[Q41] 多表连接
来源：http://hz.cucudq.cn/gthnlimlsh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.hysaishi.cn/gtvyttqspp.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhaomingkeji.xyz/gtzijoydii.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yongpay.top/gtkjlyjmfc.html

[Q42] 连接条件附加过滤
来源：http://hz.mhx1999.top/gtwguxczcb.html

SELECT u.name, o.amount FROM users u
来源：http://hz.c1oappe.top/gtpkplvuii.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.ydjk.org.cn/gtjreeitdh.html

[Q43] 标量子查询
来源：http://hz.jqgfzy.top/gtscunzcdi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.meibo888.top/gtwvwrduoa.html

[Q44] IN 子查询
来源：http://hz.cucudq.cn/gtmxgqwrsv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.aibaodan.cn/gtfsrbavsl.html

[Q45] EXISTS 判断存在
来源：http://hz.dianchejie.cn/gtitqaifft.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zdqjudy.top/gtjgzwjpmi.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.cashguo.top/gtfqpilnlu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.zhiwuduotai.top/gtuurmjxgh.html

[Q47] 与平均值比较
来源：http://hz.yangfankeji.com/gtdnjrrksm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cheryme.top/gthwnojfaj.html

[Q48] CTE 公用表表达式
来源：http://hz.cucudq.cn/gtnnifghfh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.zhaomingkeji.xyz/gtbqiadjmb.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yonumen.top/gtmxooaklh.html

[Q49] 更新单行
来源：http://hz.yuanzhike.top/gtpijzomcx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.quarkkingdee.top/gtuvjvkxik.html

[Q50] 批量更新
来源：http://hz.yj20258.top/gtdkgpvylk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jiagoushi.top/gtrczfitqc.html

[Q51] 用子查询更新
来源：http://hz.gogol.net.cn/gtijgtnbqx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.9152youxi.cn/gttkzqeuiq.html

[Q52] 删除指定行
来源：http://hz.zhiwuduotai.top/gtkrcfteyg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.sweek.top/gtyfrmwmte.html

[Q53] 按条件删除
来源：http://hz.yangfankeji.com/gtnqxbdtkr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.tianlin.xyz/gtsvxixpde.html

[Q54] 清空表
来源：http://hz.ydzc1.top/gtnrlcsbtw.html

TRUNCATE TABLE logs;
来源：http://hz.quarkkingdee.top/gtqqhujzzc.html

[Q55] 排名（并列占位）
来源：http://hz.52xcode.cn/gtfwytrcac.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.yuanzhike.top/gtqxifbxen.html

[Q56] 密集排名（并列不占位）
来源：http://hz.tianlin.xyz/gtjjsklgxq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhijiandao.cn/gtxxdnpich.html

[Q57] 行号
来源：http://hz.tianlin.xyz/gtrjqqzkyg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.aibaodan.cn/gtjltbjanb.html

[Q58] 累计求和
来源：http://hz.fzhhl.top/gtqqklblqp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.0kj1m.cn/gtqgemexty.html

[Q59] 分组内累计
来源：http://hz.tianlin.xyz/gtfrfgsjmu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.iojbl.cn/gtwjxljlsh.html

[Q60] 取上一行 / 下一行
来源：http://hz.hywenlv.cn/gthiksqajj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jianghu66.top/gtqreuljhu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhiwuduotai.top/gtqckmiwlj.html

[Q61] 移动平均
来源：http://hz.0kj1m.cn/gtmkmlfdwa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.daria6918.cn/gtgthukwkq.html

[Q62] 分组占比
来源：http://hz.ppjwa.cn/gtlgzqevex.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.9152youxi.cn/gttymcjzwj.html

[Q63] 开启事务
来源：http://hz.52xcode.cn/gtddbmvrle.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yj20258888.top/gtvjflmwzk.html

[Q64] 提交事务
来源：http://hz.guannengcc.top/gtcequfyfy.html

COMMIT;
来源：http://hz.gaohongyu789.top/gtockbbolr.html

[Q65] 回滚事务
来源：http://hz.havefunace.top/gtnmuondid.html

ROLLBACK;
来源：http://hz.yonumen.top/gttyylmkfe.html

[Q66] 行锁查询
来源：http://hz.jinqigufen.top/gtrrzikiex.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.haohaochexian.top/gtmvamdwcz.html

[Q67] 设置隔离级别
来源：http://hz.sysykeji.top/gtugvjruai.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cucudq.cn/gtxzcbnoba.html

[Q68] 保存点
来源：http://hz.aizwys.cn/gtalnyjzng.html

SAVEPOINT sp1;
来源：http://hz.sxryk.cn/gtgcdctqnm.html

ROLLBACK TO sp1;
来源：http://hz.52xcode.cn/gtzjvhdrrj.html

[Q69] 查看执行计划
来源：http://hz.meibo888.top/gtaoafevdv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.c1oappe.top/gtcdamipau.html

[Q70] 更新统计信息
来源：http://hz.yj20258.top/gtqbzdfpyy.html

ANALYZE TABLE users;
来源：http://hz.iojbl.cn/gtagfksobi.html

[Q71] 查看建表语句
来源：http://hz.daria6918.cn/gtoxrhttnv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fzhhl.top/gtchbekgqw.html

[Q72] 查看索引
来源：http://hz.xuanzx.com/gtxrapcnne.html

SHOW INDEX FROM users;
来源：http://hz.yj20258888.top/gtnjwsyetq.html

[Q73] 查看表状态
来源：http://hz.yuanzhike.top/gtzruiakyw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhengqikj.top/gtajbkxgsn.html

[Q74] 强制使用索引
来源：http://hz.zhixingplan.top/gtspdqlhdq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.pengpengdd.cyou/gtwybrlayi.html

[Q75] 日期格式化
来源：http://hz.bjfxy.top/gtsuiobuvr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.sufxvd.cn/gtgeiflnyp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jiagoushi.top/gtmzmpflft.html

[Q76] 按天统计
来源：http://hz.yuxming.cn/gtdbadnnuk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daria6918.cn/gtdjfvvabz.html

[Q77] 时间加减
来源：http://hz.jqgufenzy.top/gtrhylwbow.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinqigfzy.top/gtsmndqniv.html

[Q78] 当前时间
来源：http://hz.daria6918.cn/gtpagolfus.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtqoebyllg.html

[Q79] 字符串拼接
来源：http://hz.chenjidiqi.icu/gthtgsjoco.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yueranfly.top/gttuwxxlmq.html

[Q80] 字符串截取
来源：http://hz.hywenlv.cn/gtkursawht.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhiwuduotai.top/gtxrbrwklj.html

[Q81] 字符串替换
来源：http://hz.zycfv.cn/gtjlfgbwfr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.smart0.xyz/gtwdscoeal.html

[Q82] 字符长度与字节长度
来源：http://hz.zhoulong.xyz/gtgxwuufgd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.daxiang520.top/gtyluoksfg.html

[Q83] 大小写转换
来源：http://hz.tanke756.top/gtyfbwpajt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dashuyun.cn/gtpstltmfu.html

[Q84] 去除首尾空格
来源：http://hz.cheryme.top/gtnlgrrwcg.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhongyouzk.top/gtpxptzrnh.html

[Q85] 数值取整
来源：http://hz.9152youxi.cn/gtdjwpqomj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shanyushiyangkeji.top/gthuufdymy.html

[Q86] 读取 JSON 字段
来源：http://hz.jyoumei.cn/gtpzmwbkbh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinghuilouyu.cn/gtzugpzdmw.html

[Q87] JSON 字段做条件
来源：http://hz.yuxming.cn/gtadgqafdk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.smart0.xyz/gtgfgwcsgl.html

[Q88] 行转列（条件聚合）
来源：http://hz.shzxlz.cn/gtejnqwvog.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxinkj.top/gtnselwnwd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.nanxinkj.top/gtiqlktyae.html

[Q89] 判断表是否存在
来源：http://hz.nwbrower.top/gtelbrfvsw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gogol.net.cn/gtxpsjmlzt.html

[Q90] 生成序号列
来源：http://hz.jinqigfzy.top/gtqgsxjlid.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hongshengwenyu.top/gtonbtchhx.html

================================================================================
来源：http://hz.yonumen.top/gtsfkqauiy.html

R. Bash 专题
来源：http://hz.kuanghao11.cn/gticqarznb.html

================================================================================
来源：http://hz.guowangkeji.top/gthkiruysx.html

[R01] shebang 与严格模式
来源：http://hz.hnqzz.top/gtfxznsccu.html

#!/usr/bin/env bash
来源：http://hz.aibaodan.cn/gtwfnpensp.html

set -euo pipefail
来源：http://hz.xinyue.icu/gtztlssgps.html

[R02] 变量赋值与使用
来源：http://hz.jyoumei.cn/gttnykrezb.html

name="Tom"; echo "$name"
来源：http://hz.zhixingplan.top/gtnjgkksai.html

[R03] 只读变量
来源：http://hz.c1oappe.top/gtxyvmrbcs.html

readonly PI=3.14
来源：http://hz.zhengqikj.top/gtlxkwoasg.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gtlsymsehe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jyoumei.cn/gtdaccubiw.html

[R05] 参数默认值
来源：http://hz.vqdsnc.cn/gtqcakslql.html

name="${1:-default}"
来源：http://hz.shanyushiyangtech.top/gteuoajmwn.html

[R06] 判断命令是否存在
来源：http://hz.quarkkingdee.top/gtdktabrme.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shuidangran.top/gtwxwuliby.html

[R07] if 判断文件
来源：http://hz.bjfxy.top/gttggodgty.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj20258888.top/gthpwjemcr.html

[R08] 数值比较
来源：http://hz.zhoulong.xyz/gtzdcbjbhb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.pengpengdd.cyou/gtdfnloymy.html

[R09] 字符串比较
来源：http://hz.wangshuangyany.cn/gtyvhxlesy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.kuanghao11.cn/gtavcfirxj.html

[R10] 正则匹配
来源：http://hz.nwbrower.top/gtplnsexxc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tanke756.top/gtnfdtdbgc.html

[R11] case 多分支
来源：http://hz.feifeiyinyue.top/gtabecqljk.html

case "$1" in
来源：http://hz.ehwqpu.com/gtwfzaebur.html

start) echo "启动" ;;
来源：http://hz.havefunace.top/gteeevluio.html

stop)  echo "停止" ;;
来源：http://hz.shanyushiyangkeji.top/gtliwhhjux.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258.top/gtmwduzrni.html

esac
来源：http://hz.zycfv.cn/gtfpbzmhob.html

[R12] for 遍历文件
来源：http://hz.jinqigufen.top/gtgeibbeiw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.pycfn.com/gtmcabunwp.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtucjipqnm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xingfuxueyuan.xyz/gtqausvlyb.html

[R14] C 风格 for
来源：http://hz.zhengqikj.top/gtpabhjuml.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cheryme.top/gtvbakfmfe.html

[R15] while 逐行读文件
来源：http://hz.xinyue.icu/gtcoaltkcb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daxiang520.top/gtnmwhtbbe.html

[R16] until 等待条件
来源：http://hz.cucudq.cn/gthcuvqpzf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sweek.top/gthtkutlzf.html

[R17] 数组定义与取值
来源：http://hz.hammf.cn/gtctkenbhe.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtgftmclqb.html

[R18] 遍历数组
来源：http://hz.dianchejie.cn/gtucbylcyb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgufenzy.top/gttjfnkahk.html

[R19] 数组长度
来源：http://hz.tanke756.top/gtmkrbhcdw.html

echo "${#arr[@]}"
来源：http://hz.redwolf501.top/gtpbytrrxk.html

[R20] 关联数组（字典）
来源：http://hz.xuetiantiany.cn/gtckdzkyya.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cqqwz.cn/gttsmlzpwk.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gtxyvfdlcc.html

echo "${#s}"
来源：http://hz.feifeiyinyue.top/gtzafgoafy.html

[R22] 截取子串
来源：http://hz.nanxinkj.top/gtmdmblpvd.html

echo "${s:0:5}"
来源：http://hz.jinghuilouyu.cn/gtifhvvlzj.html

[R23] 字符串替换
来源：http://hz.yj20258888.top/gtewwadqcr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gtndswusmr.html

[R24] 大小写转换
来源：http://hz.yongpay.top/gtfeawfjla.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuanzx.com/gtugubkekc.html

[R25] 去后缀 / 去前缀
来源：http://hz.andypj.xyz/gtaattfkzz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nwbrower.top/gtijojvbir.html

[R26] 命令替换
来源：http://hz.xuanzx.com/gtfcuamotr.html

now=$(date +%F); echo "$now"
来源：http://hz.iojbl.cn/gtmarvxglr.html

[R27] 算术展开
来源：http://hz.svipenyu.cn/gtcnlwgfer.html

echo $((1 + 2 * 3))
来源：http://hz.zhaomingkeji.xyz/gteyezbfdm.html

[R28] 浮点运算
来源：http://hz.feifeiyinyue.top/gtpxlylvkd.html

echo "scale=2; 10/3" | bc
来源：http://hz.tian-w.cn/gtauzussgh.html

[R29] 定义函数
来源：http://hz.nwbrower.top/gtwlscfjca.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhaomingkeji.xyz/gtsjccegut.html

[R30] 函数返回状态码
来源：http://hz.gaohongyu789.top/gtbxctojem.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhoulong.xyz/gtxtjdtebz.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtlfpieiph.html

f() { local x=1; echo "$x"; }
来源：http://hz.redwolf501.top/gtahickfsr.html

[R32] 参数个数校验
来源：http://hz.xinyue.icu/gtrbpqbzky.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sxryk.cn/gtbrogpgcq.html

[R33] 捕获错误并提示行号
来源：http://hz.316326.xyz/gtxihaobry.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cheryme.top/gtkyafnfqr.html

[R34] 退出时清理
来源：http://hz.c1oappe.top/gtodmbnfkl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtldtyjgmf.html

[R35] 后台执行并等待
来源：http://hz.ivvv.top/gtuskvsqah.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.meibo888.top/gtsrehwuix.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtobayojjs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.andypj.xyz/gtexqvksso.html

[R37] 把输出赋给变量
来源：http://hz.ybcxt.top/gtjocozheo.html

files=$(ls -1)
来源：http://hz.daxiang520.top/gtibjyshqv.html

[R38] 管道串联
来源：http://hz.hywenlv.cn/gtzkmhbvwp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgfzy.top/gtqtzhbfmv.html

[R39] 重定向标准输出与错误
来源：http://hz.gaohongyu789.top/gtabfhkiri.html

cmd > out.log 2>&1
来源：http://hz.daria6918.cn/gtgjfyejzf.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtslppzrmn.html

echo "log" >> out.log
来源：http://hz.yj202588.top/gtdwfojldz.html

[R41] 丢弃输出
来源：http://hz.havefunace.top/gtfdqfexdu.html

cmd >/dev/null 2>&1
来源：http://hz.tian-w.cn/gtjwipysru.html

[R42] 输入重定向
来源：http://hz.dianchejie.cn/gtoxpazvvg.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gtlqdzhzag.html

[R43] 按名字查找文件
来源：http://hz.yonumen.top/gtbtmirzry.html

find . -name "*.log" -type f
来源：http://hz.hnqzz.top/gtfhinssje.html

[R44] 按修改时间查找
来源：http://hz.yueranfly.top/gtrogehjrl.html

find . -mtime -7 -type f
来源：http://hz.zhoulong.xyz/gtwxoqognh.html

[R45] 批量删除
来源：http://hz.yuanzhike.top/gtxkxtoemo.html

find . -name "*.tmp" -delete
来源：http://hz.andypj.xyz/gtpynwibzq.html

[R46] 递归替换文件内容
来源：http://hz.yj20258888.top/gtygkxisqv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xuetiantiany.cn/gtaabucnoz.html

[R47] sed 单行替换
来源：http://hz.yangfankeji.com/gtvufztlbo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.bjfxy.top/gttmxlmpco.html

[R48] awk 取指定列
来源：http://hz.jqgfzy.top/gtavcqfzxe.html

awk '{print $1, $3}' a.txt
来源：http://hz.hywenlv.cn/gtazvdjcuf.html

[R49] awk 带条件
来源：http://hz.fengsongda.top/gtkdhwcxgp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jyoumei.cn/gtggkhctnn.html

[R50] awk 求和
来源：http://hz.sxryk.cn/gtvitofqlf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtxmmpcdhr.html

[R51] 排序去重取前几
来源：http://hz.9152youxi.cn/gtlywbxfev.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.52xcode.cn/gtfhqgvyuw.html

[R52] 统计行数
来源：http://hz.ivvv.top/gtvsjdlnxg.html

wc -l a.txt
来源：http://hz.yueranfly.top/gtuvpfjktm.html

[R53] 查看文件头与实时尾
来源：http://hz.hammf.cn/gtlkzwgqei.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhijiandao.cn/gtgatghyat.html

[R54] 比较两个文件
来源：http://hz.gotoacloud.top/gtrpynuggr.html

diff a.txt b.txt
来源：http://hz.zhongyouzk.top/gtikucdqho.html

[R55] 压缩与解压
来源：http://hz.jiagoushi.top/gtdfyigwkv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gtqbjovlus.html

[R56] 远程拷贝
来源：http://hz.zycfv.cn/gtuvagvnem.html

scp file user@host:/path/
来源：http://hz.yangfankeji.com/gthwotwddb.html

[R57] 远程执行命令
来源：http://hz.kuanghao11.cn/gtmiucvaje.html

ssh user@host 'uptime'
来源：http://hz.sxryk.cn/gtuklakckn.html

[R58] 下载文件
来源：http://hz.ehwqpu.com/gtahntevdc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.havefunace.top/gttbeubkii.html

[R59] 发 POST JSON
来源：http://hz.yanxiufei.cn/gtygujteun.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xuetiantiany.cn/gtzbfenfaj.html

[R60] 只看 HTTP 状态码
来源：http://hz.hysaishi.cn/gtlqihojjc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yvedp.cn/gtxduaprrt.html

[R61] 磁盘占用
来源：http://hz.jinyuanbaomall.cn/gtobttpexa.html

df -h;  du -sh *
来源：http://hz.yj20258.top/gtlqwpelgn.html

[R62] 找最占空间的文件
来源：http://hz.9152youxi.cn/gthvtgkbrh.html

du -ah . | sort -rh | head -10
来源：http://hz.guowangkeji.top/gtgfsbbwnz.html

[R63] 内存与进程
来源：http://hz.xuanzx.com/gtdzatdqbj.html

free -h;  ps aux | grep nginx
来源：http://hz.zhixingplan.top/gtxshmsfra.html

[R64] 结束进程
来源：http://hz.hfpthk.cn/gtctbsmntv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jqgfzy.top/gtxrqagtde.html

[R65] 查看端口占用
来源：http://hz.xylfe.cn/gtzfbtovqw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.haohaochexian.top/gtmafghyhd.html

[R66] 定时任务
来源：http://hz.snrcjt.cn/gtywpvvhxh.html

crontab -e;  crontab -l
来源：http://hz.52xcode.cn/gtybkexylj.html

[R67] 生成随机十六进制串
来源：http://hz.sweek.top/gtpzntkfxb.html

openssl rand -hex 16
来源：http://hz.gogol.net.cn/gtcnojsyaw.html

[R68] 计算文件校验值
来源：http://hz.nwbrower.top/gtnndqkrkb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxuanxn.top/gtljpqpslt.html

[R69] 生成随机密码
来源：http://hz.tianlin.xyz/gtyrctzcui.html

head -c 16 /dev/urandom | base64
来源：http://hz.havefunace.top/gtkxdtjbya.html

[R70] 时间戳与互转
来源：http://hz.sysykeji.top/gtiudeysip.html

date +%s;  date -d @1700000000
来源：http://hz.cdnleiting.top/gttrqntslq.html

[R71] 日期格式化
来源：http://hz.yuxming.cn/gtgrjlandd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnqzz.top/gtjvdtplmg.html

[R72] 等待端口就绪
来源：http://hz.hywenlv.cn/gtayupaijr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.svipenyu.cn/gtcfhkjxni.html

[R73] 分割大日志
来源：http://hz.cucudq.cn/gtsombbzpu.html

split -l 1000 big.log part_
来源：http://hz.sufxvd.cn/gtlqfqspqx.html

[R74] 批量重命名
来源：http://hz.haohaochexian.top/gtxkbhdvos.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.kuanghao11.cn/gtofeorgsa.html

[R75] 导出环境变量
来源：http://hz.yuxming.cn/gtdztpamup.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.quarkkingdee.top/gtymncxznd.html

[R76] 使用临时文件
来源：http://hz.yanxiufei.cn/gtildlvnmw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtougcojwq.html

[R77] 读取用户输入
来源：http://hz.cdnleiting.top/gtwxovaksl.html


<!-- 参考信息 -->