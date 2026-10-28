代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hz.dianchejie.cn/gtfozbsouk.html

[Q26] 计数
来源：http://hz.yangfankeji.com/gtsdiwefmf.html

SELECT COUNT(*) FROM users;
来源：http://hz.smart0.xyz/gtahsqdurd.html

[Q27] 条件计数
来源：http://hz.sysykeji.top/gtydtpieur.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hz.havefunace.top/gtvtrwdxjr.html

[Q28] 求和与平均
来源：http://hz.316326.xyz/gtrpqyvxxb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hz.gaohongyu789.top/gttkeowcpg.html

[Q29] 最大最小值
来源：http://hz.zhoulong.xyz/gtufriqnrs.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://hz.zdqjudy.top/gttrkpflyl.html

[Q30] 分组统计
来源：http://hz.feifeiyinyue.top/gtciqjxfgf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hz.nanxuanxn.top/gtqhyxovzw.html

[Q31] 分组后过滤
来源：http://hz.mhx1999.top/gtzwsoniwq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.hongshengwenyu.top/gtcrikeuqw.html

[Q32] 分组拼接字符串
来源：http://hz.daria6918.cn/gtkcjpnhnv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.xziqi.cn/gtpcdkyhni.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.iojbl.cn/gtxezemikb.html

[Q33] 多列分组
来源：http://hz.jinghuilouyu.cn/gtvnmeymnu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.nanxuanxn.top/gtzvxpnztp.html

[Q34] 每组取第一条
来源：http://hz.xylfe.cn/gtdcltceqp.html

SELECT * FROM (
来源：http://hz.redwolf501.top/gtozpehllp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.ydzc1.top/gthdcvjsam.html

) t WHERE rn = 1;
来源：http://hz.jinyuanbaomall.cn/gtfrciwyzx.html

[Q35] 内连接
来源：http://hz.aizwys.cn/gtgahczrdq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.ppjwa.cn/gtgqbtkqni.html

[Q36] 左连接
来源：http://hz.hnqzz.top/gteafmdzyv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.ydjk.org.cn/gtgdtfsgcw.html

[Q37] 右连接
来源：http://hz.jinqigfzy.top/gtdkxlnfgq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.hywenlv.cn/gtqnbukdmj.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.sysykeji.top/gtoprfslmq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.nanxinkj.top/gtzfiircmy.html

[Q39] 自连接（查上下级）
来源：http://hz.meibo888.top/gtqkufzogx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.chenzaomai.com/gtwlxirmui.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.gaohongyu789.top/gtskwogamo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.cucudq.cn/gtzbibhnre.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.yuxming.cn/gtvmnaruep.html

[Q41] 多表连接
来源：http://hz.yongpay.top/gteflmxdck.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.pycfn.com/gtyxxblfsm.html

JOIN users u ON u.id = o.user_id
来源：http://hz.cqqwz.cn/gtkskwlkua.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.sxryk.cn/gttiykmaql.html

[Q42] 连接条件附加过滤
来源：http://hz.nanxuanxn.top/gtuidtsjmn.html

SELECT u.name, o.amount FROM users u
来源：http://hz.smart0.xyz/gtllhsfzkk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cqqwz.cn/gtyuyyvqqe.html

[Q43] 标量子查询
来源：http://hz.xylfe.cn/gtusdbgdmk.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.bjfxy.top/gtrbmrpvvy.html

[Q44] IN 子查询
来源：http://hz.yueranfly.top/gticsqjllp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.redwolf501.top/gtmpslgdcq.html

[Q45] EXISTS 判断存在
来源：http://hz.hnqzz.top/gthjupkete.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jinqigufen.top/gtbikfaacb.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yanxiufei.cn/gtcmtanouo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.shangyingyoupin.top/gtnxmcgmrh.html

[Q47] 与平均值比较
来源：http://hz.ydjk.org.cn/gtbkgnkzuu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.xingfuxueyuan.xyz/gthhqblehr.html

[Q48] CTE 公用表表达式
来源：http://hz.cashguo.top/gtzyeemhwy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.shanyushiyangkeji.top/gtbjsgxkdd.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.chenlongwang.top/gtbwfnwzhy.html

[Q49] 更新单行
来源：http://hz.jiagoushi.top/gtedhpnxti.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.cheryme.top/gtsjrzrduq.html

[Q50] 批量更新
来源：http://hz.tanke756.top/gtxdzcqkel.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.shzxlz.cn/gtxbrrlggh.html

[Q51] 用子查询更新
来源：http://hz.sysykeji.top/gtkcwzyaku.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.cheryme.top/gthwynhyqb.html

[Q52] 删除指定行
来源：http://hz.daria6918.cn/gtdoxhhfrc.html

DELETE FROM users WHERE id = 10;
来源：http://hz.316326.xyz/gtnriyrhoy.html

[Q53] 按条件删除
来源：http://hz.shzxlz.cn/gtqrjydoxu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cheryme.top/gtxfnmqsph.html

[Q54] 清空表
来源：http://hz.ydjk.org.cn/gtmpmvxgxd.html

TRUNCATE TABLE logs;
来源：http://hz.gzhubu.top/gtguxeudod.html

[Q55] 排名（并列占位）
来源：http://hz.yj20258.top/gtlgatiypx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ppjwa.cn/gthtgrklqk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.smart0.xyz/gtzcehpddi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yuxming.cn/gtnxjjplfe.html

[Q57] 行号
来源：http://hz.zhongyouzk.top/gtapodzvpo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgufenzy.top/gtjpggwcbl.html

[Q58] 累计求和
来源：http://hz.pengpengdd.cyou/gtocdajzos.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.aibaodan.cn/gtwfkggmxv.html

[Q59] 分组内累计
来源：http://hz.sxryk.cn/gtzxbsewze.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.fzhhl.top/gtbcdgcjkl.html

[Q60] 取上一行 / 下一行
来源：http://hz.birdmap.top/gtybaqxkfu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.tanke756.top/gtqswvzrqk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sxryk.cn/gtsanbzvbf.html

[Q61] 移动平均
来源：http://hz.yangfankeji.com/gttojzkbrb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yuxming.cn/gttewhijvi.html

[Q62] 分组占比
来源：http://hz.zdqjudy.top/gtfmlxfjvx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cdnleiting.top/gtpgccnqey.html

[Q63] 开启事务
来源：http://hz.fzhhl.top/gtzfbezkaa.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shzxlz.cn/gtzfbuaxkx.html

[Q64] 提交事务
来源：http://hz.zhixingplan.top/gtgwezjtrl.html

COMMIT;
来源：http://hz.cucudq.cn/gtfqsjyaom.html

[Q65] 回滚事务
来源：http://hz.cheryme.top/gtycgqrlbh.html

ROLLBACK;
来源：http://hz.yonumen.top/gtokpahcnt.html

[Q66] 行锁查询
来源：http://hz.sweek.top/gtwnscbjte.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.0kj1m.cn/gtpxzmemgy.html

[Q67] 设置隔离级别
来源：http://hz.52xcode.cn/gthizuzeyo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.meibo888.top/gtxtezpmui.html

[Q68] 保存点
来源：http://hz.hnxiangtu.top/gttzaltvfv.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtewvbnfqk.html

ROLLBACK TO sp1;
来源：http://hz.zdqjudy.top/gtjcgvccct.html

[Q69] 查看执行计划
来源：http://hz.hongshengwenyu.top/gtchsyjsho.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yonumen.top/gtxoudhrut.html

[Q70] 更新统计信息
来源：http://hz.guannengcc.top/gtdcectdjx.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtzejcqski.html

[Q71] 查看建表语句
来源：http://hz.yuxming.cn/gtggkigbmz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhongyouzk.top/gtztundrsr.html

[Q72] 查看索引
来源：http://hz.quarkkingdee.top/gtzexqdhkp.html

SHOW INDEX FROM users;
来源：http://hz.pycfn.com/gthedbwcpt.html

[Q73] 查看表状态
来源：http://hz.gzhubu.top/gtwdrkkfdd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.nanxinkj.top/gtcuqzonnf.html

[Q74] 强制使用索引
来源：http://hz.pycfn.com/gthljyaxvx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhengqikj.top/gtbcptarsa.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtcmuhmxbj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.tian-w.cn/gtigcxtwoj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.havefunace.top/gtmbtbnsbb.html

[Q76] 按天统计
来源：http://hz.gotoacloud.top/gtvkwbceni.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.hfpthk.cn/gtrjzlbgxr.html

[Q77] 时间加减
来源：http://hz.yueranfly.top/gtpevfwsuy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtxztxzols.html

[Q78] 当前时间
来源：http://hz.daria6918.cn/gtvgkezlrl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhijiandao.cn/gtfisyrelp.html

[Q79] 字符串拼接
来源：http://hz.jinyuanbaomall.cn/gtlmhmpbwn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.andypj.xyz/gtenwrnmxu.html

[Q80] 字符串截取
来源：http://hz.yj202588.top/gtoiqrkptp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.daxiang520.top/gtkadtivme.html

[Q81] 字符串替换
来源：http://hz.daxiang520.top/gtdnnoyqzz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxinkj.top/gtqdxffzes.html

[Q82] 字符长度与字节长度
来源：http://hz.svipenyu.cn/gtoxbdetoc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gtjknanhtp.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gtcsfexbej.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.chenjidiqi.icu/gtxrkxohux.html

[Q84] 去除首尾空格
来源：http://hz.yueranfly.top/gtdvrvdyho.html

SELECT TRIM(name) FROM users;
来源：http://hz.hywenlv.cn/gtqrvkhfgj.html

[Q85] 数值取整
来源：http://hz.zhaomingkeji.xyz/gtxcjloase.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhoulong.xyz/gtlkxigvww.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangkeji.top/gtpmnwyfmm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.tanke756.top/gtchsqgbyn.html

[Q87] JSON 字段做条件
来源：http://hz.zhixingplan.top/gtqoyeoaio.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.meibo888.top/gtjlhcbbpp.html

[Q88] 行转列（条件聚合）
来源：http://hz.xingfuxueyuan.xyz/gtizateiru.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinyuanbaomall.cn/gtjqaokqbe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gzhubu.top/gtkjdyyfkt.html

[Q89] 判断表是否存在
来源：http://hz.haohaochexian.top/gtevntkgih.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhixingplan.top/gtxfydpkvz.html

[Q90] 生成序号列
来源：http://hz.jinyuanbaomall.cn/gtdhsxxlct.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtuuvkpnmz.html

================================================================================
来源：http://hz.snrcjt.cn/gtgcxjfayp.html

R. Bash 专题
来源：http://hz.dashuyun.cn/gttbkyhfdr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtexybntrp.html

[R01] shebang 与严格模式
来源：http://hz.hysaishi.cn/gtaqfpdzxr.html

#!/usr/bin/env bash
来源：http://hz.dashuyun.cn/gtwcpgyazp.html

set -euo pipefail
来源：http://hz.hnxiangtu.top/gtrrrxcarj.html

[R02] 变量赋值与使用
来源：http://hz.hfpthk.cn/gtzuxtclog.html

name="Tom"; echo "$name"
来源：http://hz.pycfn.com/gttbrgsqlh.html

[R03] 只读变量
来源：http://hz.cheryme.top/gtkmxncfsh.html

readonly PI=3.14
来源：http://hz.xuetiantiany.cn/gtecwgycoi.html

[R04] 位置参数
来源：http://hz.52xcode.cn/gtzuyxucku.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sysykeji.top/gtzsjtlqwc.html

[R05] 参数默认值
来源：http://hz.daxiang520.top/gtypreydfs.html

name="${1:-default}"
来源：http://hz.yonumen.top/gtwpgzjmba.html

[R06] 判断命令是否存在
来源：http://hz.yvedp.cn/gtqkevgboj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fengsongda.top/gtzqdggqws.html

[R07] if 判断文件
来源：http://hz.gotoacloud.top/gtzwybqpbx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtidweapcz.html

[R08] 数值比较
来源：http://hz.shuidangran.top/gtrmaljise.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.c1oappe.top/gtgzspszzp.html

[R09] 字符串比较
来源：http://hz.jinqigufen.top/gtlkcudbhj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xziqi.cn/gtzibwfstd.html

[R10] 正则匹配
来源：http://hz.yanxiufei.cn/gtrgikaply.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.havefunace.top/gtvlcsnnnr.html

[R11] case 多分支
来源：http://hz.aizwys.cn/gtnjjxjxqs.html

case "$1" in
来源：http://hz.jqgufenzy.top/gtpkvnczem.html

start) echo "启动" ;;
来源：http://hz.52xcode.cn/gtkwhhqkna.html

stop)  echo "停止" ;;
来源：http://hz.xingfuxueyuan.xyz/gtxnjsflax.html

*)     echo "未知命令" ;;
来源：http://hz.tianlin.xyz/gtiwahbeuh.html

esac
来源：http://hz.yangfankeji.com/gtkfafxbqp.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangtech.top/gtumatcjcw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yangfankeji.com/gthlblbmze.html

[R13] for 计数循环
来源：http://hz.hnqzz.top/gtkgrpxtbv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtwrzkowtx.html

[R14] C 风格 for
来源：http://hz.sufxvd.cn/gtufdrnhmf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zdqjudy.top/gtxcfoldnx.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtnhemesge.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shangyingyoupin.top/gtigsjtotf.html

[R16] until 等待条件
来源：http://hz.mhx1999.top/gtrblwwpdn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhixingplan.top/gtesxofvoz.html

[R17] 数组定义与取值
来源：http://hz.sxryk.cn/gtjrtygruu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.guowangkeji.top/gtedtffsla.html

[R18] 遍历数组
来源：http://hz.yj202588.top/gtbskkvldv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.nanxinkj.top/gtzdwrpepm.html

[R19] 数组长度
来源：http://hz.hnqzz.top/gtehjwyzro.html

echo "${#arr[@]}"
来源：http://hz.wangdashe.top/gttpnpfqtv.html

[R20] 关联数组（字典）
来源：http://hz.yj20258.top/gtwjjjuiof.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aibaodan.cn/gtxittfoso.html

[R21] 字符串长度
来源：http://hz.cheryme.top/gtfbuescpi.html

echo "${#s}"
来源：http://hz.ywan-chungtsiang.top/gtbfimuybe.html

[R22] 截取子串
来源：http://hz.iojbl.cn/gtinnbqkeg.html

echo "${s:0:5}"
来源：http://hz.xuanzx.com/gtydpmcias.html

[R23] 字符串替换
来源：http://hz.nanxinkj.top/gtzorgvznu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sxryk.cn/gthaqygftt.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gthfvmstcl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenzaomai.com/gtmxcrzrxw.html

[R25] 去后缀 / 去前缀
来源：http://hz.dianchejie.cn/gtviqntuef.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shzxlz.cn/gtgptusplu.html

[R26] 命令替换
来源：http://hz.9152youxi.cn/gtjcvkvexn.html

now=$(date +%F); echo "$now"
来源：http://hz.xylfe.cn/gttjthubhu.html

[R27] 算术展开
来源：http://hz.0kj1m.cn/gtcfrsgtbm.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtfonaplir.html

[R28] 浮点运算
来源：http://hz.aizwys.cn/gtocddcovu.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhiwuduotai.top/gtbneiacxq.html

[R29] 定义函数
来源：http://hz.cashguo.top/gtjnbljprx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.nwbrower.top/gtuzvkdkue.html

[R30] 函数返回状态码
来源：http://hz.xuanzx.com/gtkuwnjzjx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hywenlv.cn/gtiykupgsv.html

[R31] 局部变量
来源：http://hz.gaohongyu789.top/gtmiwquibo.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangshuangyany.cn/gtorwoinvs.html

[R32] 参数个数校验
来源：http://hz.ydzc1.top/gtgtpuzjgb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hammf.cn/gteeipodbx.html

[R33] 捕获错误并提示行号
来源：http://hz.cqqwz.cn/gtlaultpne.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sweek.top/gtzeqheyir.html

[R34] 退出时清理
来源：http://hz.iojbl.cn/gtroyisnrj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtljfjfcgt.html

[R35] 后台执行并等待
来源：http://hz.nanxinkj.top/gthvpsibia.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhiwuduotai.top/gtcwocnwmw.html

[R36] 并发执行多个任务
来源：http://hz.wangdashe.top/gtgvqoyezo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cdnleiting.top/gtkjswxspo.html

[R37] 把输出赋给变量
来源：http://hz.52xcode.cn/gtwebfiwnf.html

files=$(ls -1)
来源：http://hz.yonumen.top/gtwwgyapmi.html

[R38] 管道串联
来源：http://hz.nwbrower.top/gtfzbiauex.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sysykeji.top/gtzmuogurl.html

[R39] 重定向标准输出与错误
来源：http://hz.xylfe.cn/gtljrqihuo.html

cmd > out.log 2>&1
来源：http://hz.daxiang520.top/gtrwjcwjkm.html

[R40] 追加写日志
来源：http://hz.sufxvd.cn/gtordzshck.html

echo "log" >> out.log
来源：http://hz.gzhubu.top/gtfdcmshfk.html

[R41] 丢弃输出
来源：http://hz.cqqwz.cn/gtoujftemc.html

cmd >/dev/null 2>&1
来源：http://hz.wangshuangyany.cn/gtrxetestl.html

[R42] 输入重定向
来源：http://hz.fzhhl.top/gtwerosahq.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gthkvucatg.html

[R43] 按名字查找文件
来源：http://hz.jiagoushi.top/gtnjsyiuxd.html

find . -name "*.log" -type f
来源：http://hz.jinghuilouyu.cn/gtutycacfe.html

[R44] 按修改时间查找
来源：http://hz.yvedp.cn/gtphsqgznu.html

find . -mtime -7 -type f
来源：http://hz.smart0.xyz/gtqtscovyb.html

[R45] 批量删除
来源：http://hz.jinghuilouyu.cn/gtvyrfjvrl.html

find . -name "*.tmp" -delete
来源：http://hz.gotoacloud.top/gtzttudhav.html

[R46] 递归替换文件内容
来源：http://hz.bjfxy.top/gttwirfsqn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hywenlv.cn/gtczuuwfjx.html

[R47] sed 单行替换
来源：http://hz.gotoacloud.top/gtgidxnuok.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangdashe.top/gtiqgrczka.html

[R48] awk 取指定列
来源：http://hz.shzxlz.cn/gtkaambakx.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgfzy.top/gtxhrpapic.html

[R49] awk 带条件
来源：http://hz.yangfankeji.com/gtxfupadxt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hywenlv.cn/gtsahsnkwf.html

[R50] awk 求和
来源：http://hz.ehwqpu.com/gtglssjxdz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ybcxt.top/gthpmbksej.html

[R51] 排序去重取前几
来源：http://hz.hongshengwenyu.top/gtfckjhdvf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jiagoushi.top/gtcsqtcizy.html

[R52] 统计行数
来源：http://hz.shanyushiyangtech.top/gtqpkpbaey.html

wc -l a.txt
来源：http://hz.ydjk.org.cn/gtijazufkt.html

[R53] 查看文件头与实时尾
来源：http://hz.yueranfly.top/gtbjyrfncc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tianlin.xyz/gtcznhfbgs.html

[R54] 比较两个文件
来源：http://hz.zhiwuduotai.top/gteceylzaz.html

diff a.txt b.txt
来源：http://hz.gaohongyu789.top/gtunjyqwav.html

[R55] 压缩与解压
来源：http://hz.cdnleiting.top/gtfncephls.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.daria6918.cn/gtpudifedj.html

[R56] 远程拷贝
来源：http://hz.redwolf501.top/gtadvesxzv.html

scp file user@host:/path/
来源：http://hz.smart0.xyz/gtzyguazhl.html

[R57] 远程执行命令
来源：http://hz.hnqzz.top/gttxjcwsuk.html

ssh user@host 'uptime'
来源：http://hz.yuanzhike.top/gtvgsfzind.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gthmdqalwc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.316326.xyz/gtlshiqtzc.html

[R59] 发 POST JSON
来源：http://hz.316326.xyz/gtearintoj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.9152youxi.cn/gtmwvahvnc.html

[R60] 只看 HTTP 状态码
来源：http://hz.cashguo.top/gtxdwxoeen.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cucudq.cn/gtnfvbbprk.html

[R61] 磁盘占用
来源：http://hz.wangshuangyany.cn/gtruysotmf.html

df -h;  du -sh *
来源：http://hz.jinghuilouyu.cn/gtvkiwylnc.html

[R62] 找最占空间的文件
来源：http://hz.daria6918.cn/gtzfvcaazv.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxinkj.top/gtvacsyksn.html

[R63] 内存与进程
来源：http://hz.xuanzx.com/gtmxkrssff.html

free -h;  ps aux | grep nginx
来源：http://hz.zhoulong.xyz/gtvjjovwlt.html

[R64] 结束进程
来源：http://hz.jyoumei.cn/gtedlvwslt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtdyelcymj.html

[R65] 查看端口占用
来源：http://hz.shanyushiyangtech.top/gtsigihddt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtfiviqavv.html

[R66] 定时任务
来源：http://hz.xinyue.icu/gtjaiflfrz.html

crontab -e;  crontab -l
来源：http://hz.smart0.xyz/gtyeksnjed.html

[R67] 生成随机十六进制串
来源：http://hz.haohaochexian.top/gtdhgaouql.html

openssl rand -hex 16
来源：http://hz.jinqigfzy.top/gtzvokvroy.html

[R68] 计算文件校验值
来源：http://hz.gaohongyu789.top/gtwgpakudh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jyoumei.cn/gteolyiuaq.html

[R69] 生成随机密码
来源：http://hz.cdnleiting.top/gtsqtyibxl.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtmrvvfrra.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gtexumlawk.html

date +%s;  date -d @1700000000
来源：http://hz.aizwys.cn/gtktehoyck.html

[R71] 日期格式化
来源：http://hz.dashuyun.cn/gtkfbylfru.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gtlhhqmhtu.html

[R72] 等待端口就绪
来源：http://hz.ybcxt.top/gthpidqqpz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.wangdashe.top/gtimdmpvrt.html

[R73] 分割大日志
来源：http://hz.hfpthk.cn/gtzowfoklz.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtxtnumilq.html

[R74] 批量重命名
来源：http://hz.meibo888.top/gtyucdrbcz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shanyushiyangtech.top/gtgqimblxl.html

[R75] 导出环境变量
来源：http://hz.iojbl.cn/gtlprgnrdx.html


<!-- 参考信息 -->