代发 wailian999

[Q36] 左连接
来源：http://hz.sufxvd.cn/gtvntsyyrv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.birdmap.top/gtrqkqrdjs.html

[Q37] 右连接
来源：http://hz.sysykeji.top/gtbjuiarxa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.chenjidiqi.icu/gtqvdxdjsr.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.yj20258888.top/gtivlysaff.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.haohaochexian.top/gttzneqfoh.html

[Q39] 自连接（查上下级）
来源：http://hz.mhx1999.top/gtdwendlra.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.jyoumei.cn/gtczkndlci.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.guannengcc.top/gtxceavuhs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jinqigufen.top/gtfbvosjrn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.shanyushiyangkeji.top/gtasprzuov.html

[Q41] 多表连接
来源：http://hz.yuanzhike.top/gtrolgynqm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.0kj1m.cn/gtvsdfotqd.html

JOIN users u ON u.id = o.user_id
来源：http://hz.zhixingplan.top/gtnljmpphr.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.yonumen.top/gtmpvqlftx.html

[Q42] 连接条件附加过滤
来源：http://hz.yuxming.cn/gtlygywhmm.html

SELECT u.name, o.amount FROM users u
来源：http://hz.jinghuilouyu.cn/gtdzyvmqmq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.cheryme.top/gtddhvgwhf.html

[Q43] 标量子查询
来源：http://hz.cheryme.top/gtsxyevcgd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.chenzaomai.com/gttbhqmpkg.html

[Q44] IN 子查询
来源：http://hz.yanxiufei.cn/gtgdztevzy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jlsjyb.cn/gtaqrkczzi.html

[Q45] EXISTS 判断存在
来源：http://hz.zhengqikj.top/gtbqooxbnp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.havefunace.top/gtdiaujoid.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.nwbrower.top/gtwvfybdan.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.nanxinkj.top/gtkaxvpzyi.html

[Q47] 与平均值比较
来源：http://hz.cucudq.cn/gtyvibngbu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.havefunace.top/gtrogwwazu.html

[Q48] CTE 公用表表达式
来源：http://hz.cucudq.cn/gtrstwsvsd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jlsjyb.cn/gtizofwnuu.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.daria6918.cn/gtegbqlkdb.html

[Q49] 更新单行
来源：http://hz.shanyushiyangtech.top/gtcyaaygcs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.meibo888.top/gtcoupvnuo.html

[Q50] 批量更新
来源：http://hz.sysykeji.top/gtiizcdwga.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinqigfzy.top/gtygutprte.html

[Q51] 用子查询更新
来源：http://hz.tianlin.xyz/gtkbpmmizs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gotoacloud.top/gtjksbwuhk.html

[Q52] 删除指定行
来源：http://hz.iojbl.cn/gtzholsxnl.html

DELETE FROM users WHERE id = 10;
来源：http://hz.yonumen.top/gtbkabqoex.html

[Q53] 按条件删除
来源：http://hz.xziqi.cn/gtbmlvimxk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.xuetiantiany.cn/gtqhmcqsmj.html

[Q54] 清空表
来源：http://hz.shuidangran.top/gtgyohwjao.html

TRUNCATE TABLE logs;
来源：http://hz.cdnleiting.top/gtnpfvhyyu.html

[Q55] 排名（并列占位）
来源：http://hz.havefunace.top/gtjtjpixdh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.pengpengdd.cyou/gtyxdqmrpz.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gogol.net.cn/gtdnemdupl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hnxiangtu.top/gtaaqjzwva.html

[Q57] 行号
来源：http://hz.yangfankeji.com/gtjchfpfkt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhijiandao.cn/gtgieruayw.html

[Q58] 累计求和
来源：http://hz.jinyuanbaomall.cn/gtxdwmpwgm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jianghu66.top/gttbhojtah.html

[Q59] 分组内累计
来源：http://hz.dashuyun.cn/gtrnyakkhf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jqgufenzy.top/gtkdbdpjcb.html

[Q60] 取上一行 / 下一行
来源：http://hz.snrcjt.cn/gtuyfczkdn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuanzx.com/gtoeanumap.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jlsjyb.cn/gtogppxihc.html

[Q61] 移动平均
来源：http://hz.ywan-chungtsiang.top/gtvjnfkkvt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtgdojfmok.html

[Q62] 分组占比
来源：http://hz.ydzc1.top/gtwwldnyed.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtzvufpnvj.html

[Q63] 开启事务
来源：http://hz.chenlongwang.top/gtnoeuntrs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.sufxvd.cn/gtwvsfbbkp.html

[Q64] 提交事务
来源：http://hz.chenlongwang.top/gtrkilikmj.html

COMMIT;
来源：http://hz.ehwqpu.com/gtnruzpnhs.html

[Q65] 回滚事务
来源：http://hz.havefunace.top/gtfpdkluyl.html

ROLLBACK;
来源：http://hz.havefunace.top/gtdghfghxt.html

[Q66] 行锁查询
来源：http://hz.zycfv.cn/gturjfeoht.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.aibaodan.cn/gtyznmdujj.html

[Q67] 设置隔离级别
来源：http://hz.cqqwz.cn/gtbaqyquwo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aizwys.cn/gtmniyxnco.html

[Q68] 保存点
来源：http://hz.9152youxi.cn/gtdrwgulys.html

SAVEPOINT sp1;
来源：http://hz.tian-w.cn/gtqngixndd.html

ROLLBACK TO sp1;
来源：http://hz.zhixingplan.top/gtcjzlnegh.html

[Q69] 查看执行计划
来源：http://hz.yj20258888.top/gtpnwmapjs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhengqikj.top/gtucxzlitm.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtttmivosj.html

ANALYZE TABLE users;
来源：http://hz.yangfankeji.com/gtqvomumkd.html

[Q71] 查看建表语句
来源：http://hz.redwolf501.top/gtkvmzcbys.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daxiang520.top/gtmjfopqwx.html

[Q72] 查看索引
来源：http://hz.mhx1999.top/gtiqmlcyie.html

SHOW INDEX FROM users;
来源：http://hz.pycfn.com/gtamwavjpj.html

[Q73] 查看表状态
来源：http://hz.shanyushiyangtech.top/gttfjzhbfb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.wangdashe.top/gtnwkxmazf.html

[Q74] 强制使用索引
来源：http://hz.c1oappe.top/gtkpgzixcq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xuetiantiany.cn/gtuaoxrmgj.html

[Q75] 日期格式化
来源：http://hz.tianlin.xyz/gtmhghuqqm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.mhx1999.top/gtpgljjjox.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhaomingkeji.xyz/gtcecjcptb.html

[Q76] 按天统计
来源：http://hz.jqgfzy.top/gtnyyeihwf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ydzc1.top/gteccutoky.html

[Q77] 时间加减
来源：http://hz.jiagoushi.top/gtdmeoulrd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jiagoushi.top/gtrndxeobj.html

[Q78] 当前时间
来源：http://hz.zhaomingkeji.xyz/gtfdvssdqy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pengpengdd.cyou/gtyjyfdoye.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gthuuimrtj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hammf.cn/gtscbgvhuj.html

[Q80] 字符串截取
来源：http://hz.chenzaomai.com/gtiapweujn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ivvv.top/gtboafyujm.html

[Q81] 字符串替换
来源：http://hz.daria6918.cn/gtkondwskr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.meibo888.top/gtswznezqo.html

[Q82] 字符长度与字节长度
来源：http://hz.wangdashe.top/gtafupaxrm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.birdmap.top/gttddjsskx.html

[Q83] 大小写转换
来源：http://hz.fengsongda.top/gtrflrmhxw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yonumen.top/gtxrvaurdn.html

[Q84] 去除首尾空格
来源：http://hz.hysaishi.cn/gtujheqrjd.html

SELECT TRIM(name) FROM users;
来源：http://hz.nanxuanxn.top/gtyezrtvip.html

[Q85] 数值取整
来源：http://hz.jinghuilouyu.cn/gtittpfzfh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.hysaishi.cn/gtfmkphbrh.html

[Q86] 读取 JSON 字段
来源：http://hz.smart0.xyz/gtuzxojost.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.wangshuangyany.cn/gtenmgweng.html

[Q87] JSON 字段做条件
来源：http://hz.yj20258888.top/gtcjynhrzf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guowangkeji.top/gtoqoousjn.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhongyouzk.top/gtpyfdvoxi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sysykeji.top/gteucvhnnm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jinqigufen.top/gtxpcekjwy.html

[Q89] 判断表是否存在
来源：http://hz.dashuyun.cn/gtcachssbj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zdqjudy.top/gtcgcrjher.html

[Q90] 生成序号列
来源：http://hz.jlsjyb.cn/gtjtgfdnku.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gteuupgqel.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtatpmozcm.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtgmembdxf.html

================================================================================
来源：http://hz.yonumen.top/gtotgjrdga.html

[R01] shebang 与严格模式
来源：http://hz.xziqi.cn/gtmavjofum.html

#!/usr/bin/env bash
来源：http://hz.shuidangran.top/gtmtlwdrvb.html

set -euo pipefail
来源：http://hz.cheryme.top/gtcgvgmhnv.html

[R02] 变量赋值与使用
来源：http://hz.xuetiantiany.cn/gtgxcytpvj.html

name="Tom"; echo "$name"
来源：http://hz.xuetiantiany.cn/gtxweusviq.html

[R03] 只读变量
来源：http://hz.xinyue.icu/gtpctmfjwy.html

readonly PI=3.14
来源：http://hz.daxiang520.top/gtopcmjrao.html

[R04] 位置参数
来源：http://hz.nwbrower.top/gtduthqity.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.guowangkeji.top/gtchzjpkos.html

[R05] 参数默认值
来源：http://hz.ydjk.org.cn/gtlukoiujm.html

name="${1:-default}"
来源：http://hz.tian-w.cn/gtwrjjigwz.html

[R06] 判断命令是否存在
来源：http://hz.sweek.top/gtqjsumrha.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtdntvbhon.html

[R07] if 判断文件
来源：http://hz.cucudq.cn/gtjwyamyqk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtrggfwkmm.html

[R08] 数值比较
来源：http://hz.shzxlz.cn/gtsfmfoipq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jianghu66.top/gtozdseokc.html

[R09] 字符串比较
来源：http://hz.aibaodan.cn/gtosljvrqu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydzc1.top/gtvspubcdg.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gtldgnhxri.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinyuanbaomall.cn/gtwympernf.html

[R11] case 多分支
来源：http://hz.chenzaomai.com/gtcywddnnb.html

case "$1" in
来源：http://hz.hywenlv.cn/gtwttdrsgn.html

start) echo "启动" ;;
来源：http://hz.hysaishi.cn/gtylizczxv.html

stop)  echo "停止" ;;
来源：http://hz.zhengqikj.top/gtmsaayybt.html

*)     echo "未知命令" ;;
来源：http://hz.yuxming.cn/gtgbncqejf.html

esac
来源：http://hz.cucudq.cn/gtujmazdru.html

[R12] for 遍历文件
来源：http://hz.hongshengwenyu.top/gtjqcdrwrk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtemqhemny.html

[R13] for 计数循环
来源：http://hz.52xcode.cn/gtpguyolro.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtjrofhbdb.html

[R14] C 风格 for
来源：http://hz.jqgfzy.top/gtfksxplrh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.0kj1m.cn/gtzwjwtwkg.html

[R15] while 逐行读文件
来源：http://hz.aibaodan.cn/gteavfmzff.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.havefunace.top/gtdhgucxzz.html

[R16] until 等待条件
来源：http://hz.aibaodan.cn/gtxcmzajla.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.redwolf501.top/gtudyzimyg.html

[R17] 数组定义与取值
来源：http://hz.yuanzhike.top/gtdcjxzdhd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.c1oappe.top/gttttvvfay.html

[R18] 遍历数组
来源：http://hz.yonumen.top/gtmjcusnlk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jinghuilouyu.cn/gtbxbkmhoc.html

[R19] 数组长度
来源：http://hz.ydzc1.top/gtsvqcvbxq.html

echo "${#arr[@]}"
来源：http://hz.shangyingyoupin.top/gtoqjcbspc.html

[R20] 关联数组（字典）
来源：http://hz.xylfe.cn/gtasznbraz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shangyingyoupin.top/gtjxgijjhz.html

[R21] 字符串长度
来源：http://hz.yj202588.top/gtwelsebmx.html

echo "${#s}"
来源：http://hz.shanyushiyangkeji.top/gtqaryncot.html

[R22] 截取子串
来源：http://hz.kuanghao11.cn/gtarmwhjts.html

echo "${s:0:5}"
来源：http://hz.jqgufenzy.top/gtjduxnbvh.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtjwwdpgdy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.bjfxy.top/gtgmixgzyq.html

[R24] 大小写转换
来源：http://hz.pycfn.com/gteleqhbrk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jinyuanbaomall.cn/gthuquicjc.html

[R25] 去后缀 / 去前缀
来源：http://hz.daria6918.cn/gtjrmpwzdt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zdqjudy.top/gtbsmamyzl.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gtjuaotcpw.html

now=$(date +%F); echo "$now"
来源：http://hz.snrcjt.cn/gttcrzbrjf.html

[R27] 算术展开
来源：http://hz.haohaochexian.top/gtyxeszigb.html

echo $((1 + 2 * 3))
来源：http://hz.bjfxy.top/gtdtdwrrvj.html

[R28] 浮点运算
来源：http://hz.shuidangran.top/gtplpzesnu.html

echo "scale=2; 10/3" | bc
来源：http://hz.gotoacloud.top/gtngdahhkq.html

[R29] 定义函数
来源：http://hz.guowangkeji.top/gtqbucckha.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.svipenyu.cn/gttobtdjnd.html

[R30] 函数返回状态码
来源：http://hz.xuetiantiany.cn/gtcudtldio.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cheryme.top/gtgwdlwofp.html

[R31] 局部变量
来源：http://hz.cheryme.top/gtfmornzqu.html

f() { local x=1; echo "$x"; }
来源：http://hz.kuanghao11.cn/gtaznkeqrr.html

[R32] 参数个数校验
来源：http://hz.shanyushiyangkeji.top/gtlbzszfdt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yvedp.cn/gtdfrggrhk.html

[R33] 捕获错误并提示行号
来源：http://hz.aibaodan.cn/gtqrsnkhgm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hnxiangtu.top/gtvsoaitwd.html

[R34] 退出时清理
来源：http://hz.daria6918.cn/gtkxapidhe.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yuxming.cn/gtmnzqsexl.html

[R35] 后台执行并等待
来源：http://hz.dianchejie.cn/gtvopsvfci.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigufen.top/gtnzltpvnt.html

[R36] 并发执行多个任务
来源：http://hz.redwolf501.top/gtrdxfhaor.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.quarkkingdee.top/gtflvmckwy.html

[R37] 把输出赋给变量
来源：http://hz.gogol.net.cn/gtsarhakqf.html

files=$(ls -1)
来源：http://hz.svipenyu.cn/gtahjgtgft.html

[R38] 管道串联
来源：http://hz.dashuyun.cn/gtbmowfkrg.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gtafrnpoil.html

[R39] 重定向标准输出与错误
来源：http://hz.shzxlz.cn/gtwksexeyj.html

cmd > out.log 2>&1
来源：http://hz.hfpthk.cn/gtvqocnjxj.html

[R40] 追加写日志
来源：http://hz.jqgufenzy.top/gtyxjzavmr.html

echo "log" >> out.log
来源：http://hz.pengpengdd.cyou/gtuqnzniun.html

[R41] 丢弃输出
来源：http://hz.xziqi.cn/gtltwepybg.html

cmd >/dev/null 2>&1
来源：http://hz.bjfxy.top/gtioreyvgp.html

[R42] 输入重定向
来源：http://hz.tianlin.xyz/gtukebjetm.html

wc -l < a.txt
来源：http://hz.pengpengdd.cyou/gtzyivfmyo.html

[R43] 按名字查找文件
来源：http://hz.cashguo.top/gttllrqzpd.html

find . -name "*.log" -type f
来源：http://hz.cqqwz.cn/gtwwadcngs.html

[R44] 按修改时间查找
来源：http://hz.ydzc1.top/gtqbilbxme.html

find . -mtime -7 -type f
来源：http://hz.jyoumei.cn/gtewztjiev.html

[R45] 批量删除
来源：http://hz.yanxiufei.cn/gtnmvvaikx.html

find . -name "*.tmp" -delete
来源：http://hz.xinyue.icu/gtcrtstjli.html

[R46] 递归替换文件内容
来源：http://hz.dashuyun.cn/gttyravcpy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gtndjcvzyn.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gthyxtlzaq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhengqikj.top/gtwxlhlnzf.html

[R48] awk 取指定列
来源：http://hz.shuidangran.top/gtpnpggahd.html

awk '{print $1, $3}' a.txt
来源：http://hz.daxiang520.top/gtzmjidfkl.html

[R49] awk 带条件
来源：http://hz.ppjwa.cn/gtqbjhgzde.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gtvpynsrfa.html

[R50] awk 求和
来源：http://hz.9152youxi.cn/gtrzexoqit.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shzxlz.cn/gtkyfrefwn.html

[R51] 排序去重取前几
来源：http://hz.cqqwz.cn/gtpeommqoi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinyuanbaomall.cn/gthuupblpt.html

[R52] 统计行数
来源：http://hz.fengsongda.top/gtgvdteygg.html

wc -l a.txt
来源：http://hz.hnxiangtu.top/gtjejhgzpu.html

[R53] 查看文件头与实时尾
来源：http://hz.yangfankeji.com/gtefpbrmlg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.guannengcc.top/gtiwdewcfv.html

[R54] 比较两个文件
来源：http://hz.hnxiangtu.top/gtcjlyjljy.html

diff a.txt b.txt
来源：http://hz.hysaishi.cn/gtfyyolwzy.html

[R55] 压缩与解压
来源：http://hz.yueranfly.top/gtcheyckwy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhongyouzk.top/gtvdbwulle.html

[R56] 远程拷贝
来源：http://hz.zhoulong.xyz/gttznfevvg.html

scp file user@host:/path/
来源：http://hz.jqgfzy.top/gtfxnwaaon.html

[R57] 远程执行命令
来源：http://hz.meibo888.top/gtyrhbvibl.html

ssh user@host 'uptime'
来源：http://hz.vqdsnc.cn/gtqpwihepw.html

[R58] 下载文件
来源：http://hz.gotoacloud.top/gthkaxfemc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pengpengdd.cyou/gtuenachns.html

[R59] 发 POST JSON
来源：http://hz.snrcjt.cn/gtdrdqtqnp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shzxlz.cn/gtgnngnxmg.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuanzx.com/gtdvyjglbp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cashguo.top/gthyxwctgb.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtjxerltrw.html

df -h;  du -sh *
来源：http://hz.xuanzx.com/gttxxgwuce.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtfxemjgps.html

du -ah . | sort -rh | head -10
来源：http://hz.ivvv.top/gtcgfywzik.html

[R63] 内存与进程
来源：http://hz.ybcxt.top/gthdzzusos.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgfzy.top/gtbzxwtyly.html

[R64] 结束进程
来源：http://hz.smart0.xyz/gtilsvigtj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sxryk.cn/gtxwwlnwcd.html

[R65] 查看端口占用
来源：http://hz.jinqigufen.top/gtoiaoozzr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinqigfzy.top/gtlafqnljb.html

[R66] 定时任务
来源：http://hz.zycfv.cn/gtpmpmfslu.html

crontab -e;  crontab -l
来源：http://hz.ivvv.top/gtsbzqctgo.html

[R67] 生成随机十六进制串
来源：http://hz.redwolf501.top/gtnoridnnf.html

openssl rand -hex 16
来源：http://hz.shanyushiyangtech.top/gtqqmqbnel.html

[R68] 计算文件校验值
来源：http://hz.jqgufenzy.top/gtkihymcvw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.wangdashe.top/gtjdufhsfk.html

[R69] 生成随机密码
来源：http://hz.ydjk.org.cn/gtnrbiuxea.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinghuilouyu.cn/gtgikomikm.html

[R70] 时间戳与互转
来源：http://hz.hnxiangtu.top/gtfvwyqkru.html

date +%s;  date -d @1700000000
来源：http://hz.ydjk.org.cn/gtzlkusipn.html

[R71] 日期格式化
来源：http://hz.0kj1m.cn/gtulwrlfqh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hongshengwenyu.top/gtzfsqxayh.html

[R72] 等待端口就绪
来源：http://hz.yj20258.top/gtnmrnwwoz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gtfnyjeamj.html

[R73] 分割大日志
来源：http://hz.yongpay.top/gtacrdkibw.html

split -l 1000 big.log part_
来源：http://hz.sysykeji.top/gtbmkdqzoj.html

[R74] 批量重命名
来源：http://hz.chenjidiqi.icu/gtgmnwgsag.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhaomingkeji.xyz/gtyzlrcele.html

[R75] 导出环境变量
来源：http://hz.redwolf501.top/gtenhxpvjf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ehwqpu.com/gtlrpdvzuj.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtypxpngdz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtyheuutpz.html

[R77] 读取用户输入
来源：http://hz.yuxming.cn/gtkonetzdr.html

read -rp "请输入: " ans
来源：http://hz.fzhhl.top/gtjjjxthyy.html

[R78] 交互式菜单
来源：http://hz.nanxinkj.top/gtmlolnbwq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.wangshuangyany.cn/gtojheeqmm.html

[R79] 解析命令行选项
来源：http://hz.xuanzx.com/gtandncxok.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aibaodan.cn/gtvvkebqba.html

[R80] 查看脚本执行耗时
来源：http://hz.pengpengdd.cyou/gtryaioymg.html

time ./run.sh
来源：http://hz.cqqwz.cn/gtwhfdnkmk.html

================================================================================
来源：http://hz.nwbrower.top/gtiwphlbru.html

S. C / C++ 专题
来源：http://hz.quarkkingdee.top/gtzcnvhlao.html

================================================================================
来源：http://hz.dianchejie.cn/gtdgqejxby.html

[S01] C：Hello World
来源：http://hz.tanke756.top/gtpiqnfybd.html

#include <stdio.h>
来源：http://hz.zhoulong.xyz/gtztgdctid.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhixingplan.top/gtnxdtcsbu.html

[S02] C：变量与格式化输出
来源：http://hz.dashuyun.cn/gtceulcugo.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj202588.top/gtvtfokmmu.html

[S03] C：读入整数
来源：http://hz.ywan-chungtsiang.top/gtrfvqfijs.html

int x; scanf("%d", &x);
来源：http://hz.jianghu66.top/gtqfnankpl.html

[S04] C：字符串复制
来源：http://hz.jinyuanbaomall.cn/gtueekxfos.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cqqwz.cn/gtlhiqoudt.html

[S05] C：字符串长度
来源：http://hz.wangdashe.top/gtbgzukyig.html


<!-- 参考信息 -->