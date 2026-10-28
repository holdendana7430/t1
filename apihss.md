代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hz.ybcxt.top/gtwacvjull.html

[Q32] 分组拼接字符串
来源：http://hz.mhx1999.top/gtxyxnduda.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtzzeklliv.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hz.shzxlz.cn/gtwhejxxmd.html

[Q33] 多列分组
来源：http://hz.sweek.top/gtepyiefpc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hz.xinyue.icu/gtasspssym.html

[Q34] 每组取第一条
来源：http://hz.wangshuangyany.cn/gtbbclhsco.html

SELECT * FROM (
来源：http://hz.nanxinkj.top/gtphldwwbw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.c1oappe.top/gtwnhcheru.html

) t WHERE rn = 1;
来源：http://hz.havefunace.top/gtunoajobw.html

[Q35] 内连接
来源：http://hz.pycfn.com/gtgoyemnzn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.chenjidiqi.icu/gtygkfixne.html

[Q36] 左连接
来源：http://hz.gzhubu.top/gtgjqxcuol.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.dashuyun.cn/gtjrmqsupf.html

[Q37] 右连接
来源：http://hz.andypj.xyz/gtcgzhlcde.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.zdqjudy.top/gtoecbtxhr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.pengpengdd.cyou/gtdxjsvscb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.c1oappe.top/gteqnfqydg.html

[Q39] 自连接（查上下级）
来源：http://hz.havefunace.top/gtsloaiypg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.ydjk.org.cn/gtstjpsyob.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ehwqpu.com/gtqbaalehw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jyoumei.cn/gtgjecquxb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.jlsjyb.cn/gthfyoibyl.html

[Q41] 多表连接
来源：http://hz.zycfv.cn/gtmzcgdest.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.jyoumei.cn/gtksvxacqc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.ywan-chungtsiang.top/gttuuheeqo.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.gotoacloud.top/gtzudzhfoi.html

[Q42] 连接条件附加过滤
来源：http://hz.jqgfzy.top/gtukcodxgq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.ivvv.top/gtghxlpgjq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.jqgfzy.top/gtqbaddbxa.html

[Q43] 标量子查询
来源：http://hz.guowangkeji.top/gtltvjfgog.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtxkhlkizk.html

[Q44] IN 子查询
来源：http://hz.hywenlv.cn/gtvibkckqt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.shanyushiyangkeji.top/gtbpktdmtm.html

[Q45] EXISTS 判断存在
来源：http://hz.ydjk.org.cn/gttlojqhdy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.tianlin.xyz/gthzgxauzm.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.c1oappe.top/gtehxjeugv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ehwqpu.com/gtrvcxdfci.html

[Q47] 与平均值比较
来源：http://hz.sxryk.cn/gtyzaxezbj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gaohongyu789.top/gtybtwqvsy.html

[Q48] CTE 公用表表达式
来源：http://hz.shangyingyoupin.top/gtluaufknv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.52xcode.cn/gtrwibgogm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhoulong.xyz/gtgzztzzrj.html

[Q49] 更新单行
来源：http://hz.zdqjudy.top/gtftrctosj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.dashuyun.cn/gtvkfbnsxh.html

[Q50] 批量更新
来源：http://hz.nanxinkj.top/gtmcqsghkm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.dianchejie.cn/gttlubzlnx.html

[Q51] 用子查询更新
来源：http://hz.jlsjyb.cn/gttotfxguu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.xylfe.cn/gtrsryoves.html

[Q52] 删除指定行
来源：http://hz.xuanzx.com/gtmtzeozsj.html

DELETE FROM users WHERE id = 10;
来源：http://hz.redwolf501.top/gtxgqfknmk.html

[Q53] 按条件删除
来源：http://hz.tanke756.top/gtwjtpdpfx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.yj202588.top/gtllikhvio.html

[Q54] 清空表
来源：http://hz.yuanzhike.top/gtgtpnycli.html

TRUNCATE TABLE logs;
来源：http://hz.52xcode.cn/gtuiskdxse.html

[Q55] 排名（并列占位）
来源：http://hz.gotoacloud.top/gtigriqjij.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhoulong.xyz/gtrtwxnaiv.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yuxming.cn/gtjnvncufg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.sysykeji.top/gtojubgimd.html

[Q57] 行号
来源：http://hz.daxiang520.top/gturqdchps.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.ivvv.top/gtadusggnx.html

[Q58] 累计求和
来源：http://hz.9152youxi.cn/gtemgwignu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.pengpengdd.cyou/gtfzsgaxzy.html

[Q59] 分组内累计
来源：http://hz.hnxiangtu.top/gtodamfhmo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jinghuilouyu.cn/gtlbwveunt.html

[Q60] 取上一行 / 下一行
来源：http://hz.chenjidiqi.icu/gtqtofqvps.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.gaohongyu789.top/gtalzylquo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.guowangkeji.top/gthfkswwrx.html

[Q61] 移动平均
来源：http://hz.zhoulong.xyz/gtiywjutzj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.tian-w.cn/gtjgreedzh.html

[Q62] 分组占比
来源：http://hz.shuidangran.top/gtrcnqcnez.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtvakfwhpq.html

[Q63] 开启事务
来源：http://hz.jiagoushi.top/gteqweckue.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tian-w.cn/gtcmpadzzt.html

[Q64] 提交事务
来源：http://hz.fzhhl.top/gtzetjomwy.html

COMMIT;
来源：http://hz.hywenlv.cn/gtcdwlgrvn.html

[Q65] 回滚事务
来源：http://hz.aibaodan.cn/gtmplrsmbw.html

ROLLBACK;
来源：http://hz.zycfv.cn/gtnrsxvpwn.html

[Q66] 行锁查询
来源：http://hz.ppjwa.cn/gtdxocgopl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.haohaochexian.top/gtanskmnxr.html

[Q67] 设置隔离级别
来源：http://hz.aibaodan.cn/gtybbyveav.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jiagoushi.top/gtfcpovrzg.html

[Q68] 保存点
来源：http://hz.hammf.cn/gtbwumrwgh.html

SAVEPOINT sp1;
来源：http://hz.zhixingplan.top/gtpjciaene.html

ROLLBACK TO sp1;
来源：http://hz.nwbrower.top/gttmcqdcbb.html

[Q69] 查看执行计划
来源：http://hz.0kj1m.cn/gthxywsnsc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.gogol.net.cn/gtjkqwwrdf.html

[Q70] 更新统计信息
来源：http://hz.yj20258888.top/gtsepapvig.html

ANALYZE TABLE users;
来源：http://hz.zdqjudy.top/gtewdxcfaq.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtstucepmu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yanxiufei.cn/gtxjrwokbi.html

[Q72] 查看索引
来源：http://hz.zdqjudy.top/gtfzjoxfww.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gtpdisegsz.html

[Q73] 查看表状态
来源：http://hz.daxiang520.top/gtzsqyihzm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gzhubu.top/gtealkirgo.html

[Q74] 强制使用索引
来源：http://hz.ehwqpu.com/gttccevmyr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ywan-chungtsiang.top/gtbgosnpnm.html

[Q75] 日期格式化
来源：http://hz.jinyuanbaomall.cn/gtuxyvkwsw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gzhubu.top/gtxetktuhh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pengpengdd.cyou/gtdfwhemoz.html

[Q76] 按天统计
来源：http://hz.sysykeji.top/gtdfvejzle.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yueranfly.top/gtjawqwcuc.html

[Q77] 时间加减
来源：http://hz.xuanzx.com/gtxxpzaape.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yj20258.top/gtnejmchtr.html

[Q78] 当前时间
来源：http://hz.chenzaomai.com/gtihjfzoxa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fzhhl.top/gtdbvinios.html

[Q79] 字符串拼接
来源：http://hz.quarkkingdee.top/gttzgnocsb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.sufxvd.cn/gtpdmzybkl.html

[Q80] 字符串截取
来源：http://hz.cheryme.top/gtlsbaanhz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ybcxt.top/gtmzgefzql.html

[Q81] 字符串替换
来源：http://hz.meibo888.top/gtrtzivgds.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guannengcc.top/gtwqkntouu.html

[Q82] 字符长度与字节长度
来源：http://hz.wangshuangyany.cn/gtjyfoawae.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.gogol.net.cn/gtxjsyuium.html

[Q83] 大小写转换
来源：http://hz.sysykeji.top/gtzxufkouy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sufxvd.cn/gtjqfjvyrw.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtzqtlpktm.html

SELECT TRIM(name) FROM users;
来源：http://hz.nwbrower.top/gtsrtputos.html

[Q85] 数值取整
来源：http://hz.dashuyun.cn/gtnnibgytx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shangyingyoupin.top/gtehhgjjqj.html

[Q86] 读取 JSON 字段
来源：http://hz.sxryk.cn/gtxijpykkv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yj20258888.top/gtaakpdnns.html

[Q87] JSON 字段做条件
来源：http://hz.jqgufenzy.top/gtwpaglrny.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xylfe.cn/gtrxttnjcu.html

[Q88] 行转列（条件聚合）
来源：http://hz.jqgfzy.top/gtxhmobcvo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hnqzz.top/gtvooacoak.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.guowangkeji.top/gtarijdzvw.html

[Q89] 判断表是否存在
来源：http://hz.cashguo.top/gtpfodzqne.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daxiang520.top/gtfeuwkeit.html

[Q90] 生成序号列
来源：http://hz.svipenyu.cn/gtckaysptd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tian-w.cn/gtorjchbxp.html

================================================================================
来源：http://hz.zhengqikj.top/gtkafyrdmc.html

R. Bash 专题
来源：http://hz.quarkkingdee.top/gthgonzydk.html

================================================================================
来源：http://hz.cheryme.top/gtpdqqhgkj.html

[R01] shebang 与严格模式
来源：http://hz.aibaodan.cn/gtgzrrlmac.html

#!/usr/bin/env bash
来源：http://hz.yuxming.cn/gtwphmlrxh.html

set -euo pipefail
来源：http://hz.dianchejie.cn/gtmuzclvhk.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gtpxwhdcit.html

name="Tom"; echo "$name"
来源：http://hz.dianchejie.cn/gthxnaprqr.html

[R03] 只读变量
来源：http://hz.shangyingyoupin.top/gtpphdwffs.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtfhunjauq.html

[R04] 位置参数
来源：http://hz.hywenlv.cn/gtebhrkjmu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.guowangkeji.top/gtlzyfojvq.html

[R05] 参数默认值
来源：http://hz.wangshuangyany.cn/gtlljxkjqm.html

name="${1:-default}"
来源：http://hz.ywan-chungtsiang.top/gtccxonzcd.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gtsvufqidh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.vqdsnc.cn/gtxkbuegrg.html

[R07] if 判断文件
来源：http://hz.xylfe.cn/gtctyrqgxq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.quarkkingdee.top/gtjmgosyvs.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gtazllqivm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dianchejie.cn/gttdhmvpuy.html

[R09] 字符串比较
来源：http://hz.0kj1m.cn/gtxmqwegcw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.svipenyu.cn/gtggwwjrlm.html

[R10] 正则匹配
来源：http://hz.hongshengwenyu.top/gtmageblqd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cdnleiting.top/gtpjxzvsyh.html

[R11] case 多分支
来源：http://hz.aibaodan.cn/gtoqvsjkun.html

case "$1" in
来源：http://hz.shangyingyoupin.top/gtnjnqfujm.html

start) echo "启动" ;;
来源：http://hz.birdmap.top/gteydttciw.html

stop)  echo "停止" ;;
来源：http://hz.316326.xyz/gthdnerdpf.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtxuwmzzoz.html

esac
来源：http://hz.ivvv.top/gtfvdpzptn.html

[R12] for 遍历文件
来源：http://hz.tian-w.cn/gtjfeyuxif.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yangfankeji.com/gtpwbedhip.html

[R13] for 计数循环
来源：http://hz.meibo888.top/gtqxwctmrq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtwgelqsvj.html

[R14] C 风格 for
来源：http://hz.birdmap.top/gtyhjzayyn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shzxlz.cn/gtxkzuhicy.html

[R15] while 逐行读文件
来源：http://hz.ybcxt.top/gtzscqstwb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigufen.top/gtkxauatub.html

[R16] until 等待条件
来源：http://hz.dianchejie.cn/gtbxszebas.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.havefunace.top/gtndriljqn.html

[R17] 数组定义与取值
来源：http://hz.hnxiangtu.top/gtxvqyrdwn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj202588.top/gtahvjbwrw.html

[R18] 遍历数组
来源：http://hz.fzhhl.top/gtpkstdign.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shuidangran.top/gtvhbatuzc.html

[R19] 数组长度
来源：http://hz.tanke756.top/gtaolfxqnh.html

echo "${#arr[@]}"
来源：http://hz.c1oappe.top/gtkiadzyqm.html

[R20] 关联数组（字典）
来源：http://hz.jinqigufen.top/gtbpwkohou.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.guowangkeji.top/gtgtchhxdh.html

[R21] 字符串长度
来源：http://hz.ybcxt.top/gtlfxytdrg.html

echo "${#s}"
来源：http://hz.chenzaomai.com/gtqdhnegxo.html

[R22] 截取子串
来源：http://hz.9152youxi.cn/gtppkipfak.html

echo "${s:0:5}"
来源：http://hz.birdmap.top/gtteczzkyr.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gthqggclmt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shzxlz.cn/gtilvhysxh.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gtaznlxzki.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xziqi.cn/gtdahnmyet.html

[R25] 去后缀 / 去前缀
来源：http://hz.meibo888.top/gtinqjebok.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.52xcode.cn/gtvqcaeqvr.html

[R26] 命令替换
来源：http://hz.zdqjudy.top/gtweawctjd.html

now=$(date +%F); echo "$now"
来源：http://hz.fengsongda.top/gtgpxtynqn.html

[R27] 算术展开
来源：http://hz.cqqwz.cn/gtqwjjnxet.html

echo $((1 + 2 * 3))
来源：http://hz.dashuyun.cn/gtmrvdjlcb.html

[R28] 浮点运算
来源：http://hz.zhiwuduotai.top/gtkatqmvqj.html

echo "scale=2; 10/3" | bc
来源：http://hz.yvedp.cn/gtsqvjcnwl.html

[R29] 定义函数
来源：http://hz.zhoulong.xyz/gtsaipmugo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.52xcode.cn/gtesqysecw.html

[R30] 函数返回状态码
来源：http://hz.iojbl.cn/gtejaaefgu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hammf.cn/gthzyvfwqt.html

[R31] 局部变量
来源：http://hz.zhiwuduotai.top/gtshodtuvs.html

f() { local x=1; echo "$x"; }
来源：http://hz.kuanghao11.cn/gtffqfvzus.html

[R32] 参数个数校验
来源：http://hz.9152youxi.cn/gtqyotirmr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtsewrqjmm.html

[R33] 捕获错误并提示行号
来源：http://hz.haohaochexian.top/gtuusyjsgo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cucudq.cn/gthjpvcjdx.html

[R34] 退出时清理
来源：http://hz.meibo888.top/gtotpfsvdw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtdogirxts.html

[R35] 后台执行并等待
来源：http://hz.nanxinkj.top/gtjossnrmd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jianghu66.top/gtcedwynhl.html

[R36] 并发执行多个任务
来源：http://hz.feifeiyinyue.top/gtxgolwraf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yangfankeji.com/gtxsjcpuyg.html

[R37] 把输出赋给变量
来源：http://hz.havefunace.top/gtaoqyvzrm.html

files=$(ls -1)
来源：http://hz.hnqzz.top/gthktotyrp.html

[R38] 管道串联
来源：http://hz.zycfv.cn/gtqduargph.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daria6918.cn/gtmvertsmf.html

[R39] 重定向标准输出与错误
来源：http://hz.jinyuanbaomall.cn/gtsrgwgzix.html

cmd > out.log 2>&1
来源：http://hz.bjfxy.top/gtgxjbmbns.html

[R40] 追加写日志
来源：http://hz.yanxiufei.cn/gtajrmgoje.html

echo "log" >> out.log
来源：http://hz.tianlin.xyz/gtkyfkoluc.html

[R41] 丢弃输出
来源：http://hz.fzhhl.top/gttqjahgel.html

cmd >/dev/null 2>&1
来源：http://hz.zdqjudy.top/gtgppcvnhk.html

[R42] 输入重定向
来源：http://hz.52xcode.cn/gtdbdnlmor.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtchudrrmw.html

[R43] 按名字查找文件
来源：http://hz.jinyuanbaomall.cn/gtyeuzkmoe.html

find . -name "*.log" -type f
来源：http://hz.zhengqikj.top/gtcckswxve.html

[R44] 按修改时间查找
来源：http://hz.yangfankeji.com/gtkckgomuy.html

find . -mtime -7 -type f
来源：http://hz.xylfe.cn/gtieiwptms.html

[R45] 批量删除
来源：http://hz.cheryme.top/gtyevimtyj.html

find . -name "*.tmp" -delete
来源：http://hz.gaohongyu789.top/gtetjhkjna.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangtech.top/gtoexdfjih.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.redwolf501.top/gtghjrchic.html

[R47] sed 单行替换
来源：http://hz.feifeiyinyue.top/gtmidkpsfl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yvedp.cn/gtqluzmxnr.html

[R48] awk 取指定列
来源：http://hz.iojbl.cn/gtaprzsqtv.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigufen.top/gtnifjivgq.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtajewvygo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guowangkeji.top/gtmmcqquzk.html

[R50] awk 求和
来源：http://hz.jqgfzy.top/gttgmdvulm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhoulong.xyz/gtpjryjkdp.html

[R51] 排序去重取前几
来源：http://hz.bjfxy.top/gtttlypdsc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnqzz.top/gttrghmcds.html

[R52] 统计行数
来源：http://hz.wangshuangyany.cn/gtliqhfnka.html

wc -l a.txt
来源：http://hz.hywenlv.cn/gtgeaiirkn.html

[R53] 查看文件头与实时尾
来源：http://hz.zhoulong.xyz/gtwevawlcl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.fzhhl.top/gtptuugbtr.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gtficcfkkg.html

diff a.txt b.txt
来源：http://hz.yanxiufei.cn/gtzbpdzfaj.html

[R55] 压缩与解压
来源：http://hz.xingfuxueyuan.xyz/gtlualcebz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.bjfxy.top/gttdivocwl.html

[R56] 远程拷贝
来源：http://hz.sxryk.cn/gtosiqkvut.html

scp file user@host:/path/
来源：http://hz.sxryk.cn/gtlkiusfry.html

[R57] 远程执行命令
来源：http://hz.jinqigufen.top/gtsjrpizey.html

ssh user@host 'uptime'
来源：http://hz.yanxiufei.cn/gtchzwvxip.html

[R58] 下载文件
来源：http://hz.birdmap.top/gtdppxxcvs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnqzz.top/gtvdbwzrem.html

[R59] 发 POST JSON
来源：http://hz.ivvv.top/gtqgjafyic.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtuukrtdvm.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj202588.top/gttfiqrhfv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.meibo888.top/gthofrhtzu.html

[R61] 磁盘占用
来源：http://hz.ydzc1.top/gtaichrurk.html

df -h;  du -sh *
来源：http://hz.hnxiangtu.top/gtalycisos.html

[R62] 找最占空间的文件
来源：http://hz.zhoulong.xyz/gtdhylwetl.html

du -ah . | sort -rh | head -10
来源：http://hz.hywenlv.cn/gtdrcjkntz.html

[R63] 内存与进程
来源：http://hz.zycfv.cn/gtcjnvqjhn.html

free -h;  ps aux | grep nginx
来源：http://hz.jyoumei.cn/gtdyrlaery.html

[R64] 结束进程
来源：http://hz.zhengqikj.top/gtsuabnfwd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.quarkkingdee.top/gtsxmdniwh.html

[R65] 查看端口占用
来源：http://hz.316326.xyz/gtvkqfbacb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sufxvd.cn/gtxysqoyam.html

[R66] 定时任务
来源：http://hz.tian-w.cn/gtqfsverte.html

crontab -e;  crontab -l
来源：http://hz.xuetiantiany.cn/gtgamqoohs.html

[R67] 生成随机十六进制串
来源：http://hz.daria6918.cn/gtwjvbxtmp.html

openssl rand -hex 16
来源：http://hz.c1oappe.top/gtiuinsjgy.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtrlquurcz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.snrcjt.cn/gtiuoczwoi.html

[R69] 生成随机密码
来源：http://hz.ivvv.top/gtwlpepwle.html

head -c 16 /dev/urandom | base64
来源：http://hz.sxryk.cn/gtgoqexqcm.html

[R70] 时间戳与互转
来源：http://hz.hfpthk.cn/gtkzqxhelp.html

date +%s;  date -d @1700000000
来源：http://hz.zdqjudy.top/gtrsbuejhk.html

[R71] 日期格式化
来源：http://hz.havefunace.top/gtljjurkhq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daria6918.cn/gtwqprxgtd.html

[R72] 等待端口就绪
来源：http://hz.tian-w.cn/gtaqvifgdz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gttejhnkmd.html

[R73] 分割大日志
来源：http://hz.ydjk.org.cn/gtcujidzsb.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gtukwdwqwe.html

[R74] 批量重命名
来源：http://hz.shangyingyoupin.top/gtyjtilury.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenjidiqi.icu/gtkwdugsxl.html

[R75] 导出环境变量
来源：http://hz.mhx1999.top/gtoymzhzqy.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shzxlz.cn/gtyueiqbnc.html

[R76] 使用临时文件
来源：http://hz.hnqzz.top/gtmspdcdjy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtpqhraqht.html

[R77] 读取用户输入
来源：http://hz.ybcxt.top/gtcduebifx.html

read -rp "请输入: " ans
来源：http://hz.dashuyun.cn/gtuixwhnel.html

[R78] 交互式菜单
来源：http://hz.ybcxt.top/gtmwofsvwq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxinkj.top/gtiwobshnd.html

[R79] 解析命令行选项
来源：http://hz.chenlongwang.top/gtznjshbgn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinqigfzy.top/gtvlklcunr.html

[R80] 查看脚本执行耗时
来源：http://hz.cucudq.cn/gtnstbeuap.html

time ./run.sh
来源：http://hz.guowangkeji.top/gtyoqpndjj.html

================================================================================
来源：http://hz.yvedp.cn/gtbqxgtydz.html


<!-- 参考信息 -->