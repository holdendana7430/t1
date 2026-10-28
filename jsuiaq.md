代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hz.cucudq.cn/gtiohfmatm.html

) t WHERE rn = 1;
来源：http://hz.zhiwuduotai.top/gtmqsvxpzh.html

[Q35] 内连接
来源：http://hz.yj20258888.top/gtylkobxuu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hz.xziqi.cn/gtvyvcqvie.html

[Q36] 左连接
来源：http://hz.yueranfly.top/gtmagaczaj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hz.svipenyu.cn/gtizgqhcsa.html

[Q37] 右连接
来源：http://hz.xingfuxueyuan.xyz/gtpveazngt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hz.shanyushiyangkeji.top/gtwxhtbmrp.html

[Q38] 全外连接（PostgreSQL）
来源：http://hz.redwolf501.top/gttvhuulse.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.gzhubu.top/gtkbmqsird.html

[Q39] 自连接（查上下级）
来源：http://hz.redwolf501.top/gtwsaaqwpy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.yongpay.top/gtpqutcljf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yueranfly.top/gtmlcyxpcc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.nanxuanxn.top/gtqzkxtldo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pengpengdd.cyou/gtwapbzhvd.html

[Q41] 多表连接
来源：http://hz.xuetiantiany.cn/gtqvrxaaso.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.xuetiantiany.cn/gtfsaddeap.html

JOIN users u ON u.id = o.user_id
来源：http://hz.smart0.xyz/gtjurrodbf.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zhixingplan.top/gtxkbudyos.html

[Q42] 连接条件附加过滤
来源：http://hz.nwbrower.top/gtdiwlehzy.html

SELECT u.name, o.amount FROM users u
来源：http://hz.hongshengwenyu.top/gtcftqetjg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shzxlz.cn/gtvagwgyog.html

[Q43] 标量子查询
来源：http://hz.yvedp.cn/gtbylacxnt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.xylfe.cn/gtmgqizqmr.html

[Q44] IN 子查询
来源：http://hz.feifeiyinyue.top/gtecdnxhdd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jqgufenzy.top/gtvlowjpco.html

[Q45] EXISTS 判断存在
来源：http://hz.zhaomingkeji.xyz/gtgnxsnnws.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtnxtvypik.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.shuidangran.top/gtzevtznzu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.ydjk.org.cn/gtrdvuknde.html

[Q47] 与平均值比较
来源：http://hz.chenlongwang.top/gtdisqfjfv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.cheryme.top/gtyvskaqft.html

[Q48] CTE 公用表表达式
来源：http://hz.c1oappe.top/gtohfqlvvy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.aibaodan.cn/gttehesuvf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.jinqigfzy.top/gtvvyrqgnn.html

[Q49] 更新单行
来源：http://hz.yongpay.top/gtqrhkbacb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.gzhubu.top/gtixvqocta.html

[Q50] 批量更新
来源：http://hz.gaohongyu789.top/gtjqkncfio.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jiagoushi.top/gtrmgydier.html

[Q51] 用子查询更新
来源：http://hz.hongshengwenyu.top/gtnnhmsaho.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.pengpengdd.cyou/gtqdcprogn.html

[Q52] 删除指定行
来源：http://hz.meibo888.top/gttuhxelcp.html

DELETE FROM users WHERE id = 10;
来源：http://hz.kuanghao11.cn/gtpjocezda.html

[Q53] 按条件删除
来源：http://hz.chenzaomai.com/gtlsfalzzo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cucudq.cn/gtjajoebyp.html

[Q54] 清空表
来源：http://hz.tanke756.top/gtgmymtmak.html

TRUNCATE TABLE logs;
来源：http://hz.yuanzhike.top/gtxlkiurjm.html

[Q55] 排名（并列占位）
来源：http://hz.aizwys.cn/gtbzfemprt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.0kj1m.cn/gtgizbkgmw.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yuxming.cn/gtjqppfggk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xinyue.icu/gtushjzdvn.html

[Q57] 行号
来源：http://hz.zhaomingkeji.xyz/gtyjikmjho.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.0kj1m.cn/gtucnnlqmv.html

[Q58] 累计求和
来源：http://hz.gogol.net.cn/gtviktckcf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.redwolf501.top/gtxkiwoakz.html

[Q59] 分组内累计
来源：http://hz.yueranfly.top/gtqfrutlpg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.iojbl.cn/gtmmivipap.html

[Q60] 取上一行 / 下一行
来源：http://hz.xuetiantiany.cn/gtpnublcol.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.hongshengwenyu.top/gthuybtveh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.havefunace.top/gtxhktfrfu.html

[Q61] 移动平均
来源：http://hz.c1oappe.top/gtjrpdsdax.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.smart0.xyz/gtcyfbdhvq.html

[Q62] 分组占比
来源：http://hz.tian-w.cn/gtwsduvnef.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.pycfn.com/gtlaokuzxh.html

[Q63] 开启事务
来源：http://hz.xingfuxueyuan.xyz/gtjxvkxcut.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigufen.top/gtcoqhabdi.html

[Q64] 提交事务
来源：http://hz.snrcjt.cn/gtwxceroau.html

COMMIT;
来源：http://hz.guannengcc.top/gttqgpoapy.html

[Q65] 回滚事务
来源：http://hz.birdmap.top/gtptzpztta.html

ROLLBACK;
来源：http://hz.bjfxy.top/gtkquqsdpi.html

[Q66] 行锁查询
来源：http://hz.zycfv.cn/gtkxyvbigo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.smart0.xyz/gtszqcucux.html

[Q67] 设置隔离级别
来源：http://hz.0kj1m.cn/gtuqnljqnw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aibaodan.cn/gtwfooigzq.html

[Q68] 保存点
来源：http://hz.zhoulong.xyz/gtcgystsks.html

SAVEPOINT sp1;
来源：http://hz.jqgufenzy.top/gtpyfmtdnf.html

ROLLBACK TO sp1;
来源：http://hz.shzxlz.cn/gtfczwabgh.html

[Q69] 查看执行计划
来源：http://hz.cashguo.top/gtknsxjaed.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fengsongda.top/gtrmitfuag.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gtvmupezgx.html

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gtadmifnjz.html

[Q71] 查看建表语句
来源：http://hz.cdnleiting.top/gtkjummqbg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenzaomai.com/gtzufbdiot.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtehdliwcj.html

SHOW INDEX FROM users;
来源：http://hz.daxiang520.top/gthfkjycbi.html

[Q73] 查看表状态
来源：http://hz.sufxvd.cn/gtdowpfuaj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.snrcjt.cn/gtntqvfxzr.html

[Q74] 强制使用索引
来源：http://hz.hywenlv.cn/gtscypicwd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.0kj1m.cn/gtboafpnec.html

[Q75] 日期格式化
来源：http://hz.fzhhl.top/gtzkahrpkz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.wangdashe.top/gtulguyzig.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxinkj.top/gtbumjjref.html

[Q76] 按天统计
来源：http://hz.cucudq.cn/gtbexcajys.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.0kj1m.cn/gthzwamxfw.html

[Q77] 时间加减
来源：http://hz.pycfn.com/gtdqxxfrfp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.yvedp.cn/gtzcndebtn.html

[Q78] 当前时间
来源：http://hz.c1oappe.top/gtyqkyemxe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhijiandao.cn/gtxwsctayl.html

[Q79] 字符串拼接
来源：http://hz.hysaishi.cn/gtawvtmjhq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangkeji.top/gtnflakuhr.html

[Q80] 字符串截取
来源：http://hz.tianlin.xyz/gtyivihjiq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cashguo.top/gthwpuwbig.html

[Q81] 字符串替换
来源：http://hz.tian-w.cn/gtsfmunctq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dianchejie.cn/gtfcdyniwd.html

[Q82] 字符长度与字节长度
来源：http://hz.cdnleiting.top/gtqswejtht.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhengqikj.top/gteaixyfud.html

[Q83] 大小写转换
来源：http://hz.havefunace.top/gttbbwwrgt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258.top/gtqmofjstu.html

[Q84] 去除首尾空格
来源：http://hz.hnqzz.top/gtvqzhkogv.html

SELECT TRIM(name) FROM users;
来源：http://hz.sxryk.cn/gtlnebxzxe.html

[Q85] 数值取整
来源：http://hz.nanxinkj.top/gtyhlhmznb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtaiserqql.html

[Q86] 读取 JSON 字段
来源：http://hz.chenjidiqi.icu/gtninnmwkr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhongyouzk.top/gttolpluop.html

[Q87] JSON 字段做条件
来源：http://hz.svipenyu.cn/gtnjeczpcz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhijiandao.cn/gtsrfwenqv.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigufen.top/gtrjowmnyd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtltuelgdb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jlsjyb.cn/gtwdaaxheq.html

[Q89] 判断表是否存在
来源：http://hz.xylfe.cn/gtcsalhiew.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.316326.xyz/gtwxobqcdr.html

[Q90] 生成序号列
来源：http://hz.jlsjyb.cn/gtnghmpela.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.dashuyun.cn/gtuachbotb.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtfmqkcduy.html

R. Bash 专题
来源：http://hz.pengpengdd.cyou/gtbrbccdly.html

================================================================================
来源：http://hz.xuetiantiany.cn/gthlujvdnv.html

[R01] shebang 与严格模式
来源：http://hz.ybcxt.top/gtgpahvmpc.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtmdjbrutz.html

set -euo pipefail
来源：http://hz.sysykeji.top/gtvcncqksl.html

[R02] 变量赋值与使用
来源：http://hz.yueranfly.top/gtdizpghig.html

name="Tom"; echo "$name"
来源：http://hz.cdnleiting.top/gtnnydcnln.html

[R03] 只读变量
来源：http://hz.aizwys.cn/gtzzvqcvgv.html

readonly PI=3.14
来源：http://hz.jyoumei.cn/gtelnooqsv.html

[R04] 位置参数
来源：http://hz.xziqi.cn/gtaasmgefy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinyuanbaomall.cn/gtxrkkatyp.html

[R05] 参数默认值
来源：http://hz.mhx1999.top/gtpdnsshce.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtzfnlvxqr.html

[R06] 判断命令是否存在
来源：http://hz.meibo888.top/gttbgudgwx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinqigfzy.top/gtkjiviflf.html

[R07] if 判断文件
来源：http://hz.guowangkeji.top/gtwofzfjdu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shuidangran.top/gtmbegeyrm.html

[R08] 数值比较
来源：http://hz.tian-w.cn/gtclybvzmt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangkeji.top/gtblxroiay.html

[R09] 字符串比较
来源：http://hz.tanke756.top/gtdodpwhqv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xylfe.cn/gtotoudtig.html

[R10] 正则匹配
来源：http://hz.nanxinkj.top/gtoilxtrhf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nanxuanxn.top/gtedkoogln.html

[R11] case 多分支
来源：http://hz.snrcjt.cn/gttwfqbmvf.html

case "$1" in
来源：http://hz.havefunace.top/gtgkuipcpf.html

start) echo "启动" ;;
来源：http://hz.jyoumei.cn/gtntmaxvxk.html

stop)  echo "停止" ;;
来源：http://hz.dashuyun.cn/gtsitediva.html

*)     echo "未知命令" ;;
来源：http://hz.guowangkeji.top/gtjzpboqwg.html

esac
来源：http://hz.gaohongyu789.top/gtuvpzhzoi.html

[R12] for 遍历文件
来源：http://hz.xziqi.cn/gttkapafno.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hammf.cn/gtqlosljxb.html

[R13] for 计数循环
来源：http://hz.cucudq.cn/gterljjwtv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yueranfly.top/gtyvtwsjnk.html

[R14] C 风格 for
来源：http://hz.wangdashe.top/gtcsujcpxh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.haohaochexian.top/gtuxkmrdwl.html

[R15] while 逐行读文件
来源：http://hz.sufxvd.cn/gtfgfuhzzv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xingfuxueyuan.xyz/gtinkzvwoy.html

[R16] until 等待条件
来源：http://hz.havefunace.top/gtkgnuqocf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sufxvd.cn/gtfaqsqlrc.html

[R17] 数组定义与取值
来源：http://hz.wangdashe.top/gtajkjfxvi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydjk.org.cn/gtqcgvrxyu.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtktoswgei.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ydjk.org.cn/gtabyqhdwv.html

[R19] 数组长度
来源：http://hz.jianghu66.top/gtpnqmcjcf.html

echo "${#arr[@]}"
来源：http://hz.yangfankeji.com/gtaqkmeike.html

[R20] 关联数组（字典）
来源：http://hz.xuanzx.com/gtmdkosfaf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhiwuduotai.top/gtuklsjfad.html

[R21] 字符串长度
来源：http://hz.sxryk.cn/gtyaxjhlrf.html

echo "${#s}"
来源：http://hz.haohaochexian.top/gtkljprivf.html

[R22] 截取子串
来源：http://hz.kuanghao11.cn/gtfzntmbvi.html

echo "${s:0:5}"
来源：http://hz.ybcxt.top/gtsyyhqgfi.html

[R23] 字符串替换
来源：http://hz.mhx1999.top/gtywqlddka.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ydjk.org.cn/gtzohuynou.html

[R24] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtciixvadl.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xziqi.cn/gtefnhrfqd.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258.top/gtcqejyogu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangshuangyany.cn/gtvzmhmoiy.html

[R26] 命令替换
来源：http://hz.chenlongwang.top/gtekghgzww.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtvfczszzr.html

[R27] 算术展开
来源：http://hz.andypj.xyz/gtydptcbuz.html

echo $((1 + 2 * 3))
来源：http://hz.dianchejie.cn/gtkwzumdtz.html

[R28] 浮点运算
来源：http://hz.shangyingyoupin.top/gttdfsnivn.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gtyaoswjcv.html

[R29] 定义函数
来源：http://hz.shanyushiyangtech.top/gtigtzdlxl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuanzhike.top/gtpaioftnw.html

[R30] 函数返回状态码
来源：http://hz.nanxuanxn.top/gtxcgjkliy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.vqdsnc.cn/gtmjierdlx.html

[R31] 局部变量
来源：http://hz.xuetiantiany.cn/gtprxhpuhc.html

f() { local x=1; echo "$x"; }
来源：http://hz.cdnleiting.top/gtnpodezpi.html

[R32] 参数个数校验
来源：http://hz.shuidangran.top/gturprqsia.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtjvicppcx.html

[R33] 捕获错误并提示行号
来源：http://hz.haohaochexian.top/gtlghunbkc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nwbrower.top/gtyrapjaio.html

[R34] 退出时清理
来源：http://hz.daxiang520.top/gtangeexvg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtipupcwqt.html

[R35] 后台执行并等待
来源：http://hz.cashguo.top/gtnzckjjhb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ydzc1.top/gtarzziley.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtkxwnhgib.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fzhhl.top/gtuxytkwdv.html

[R37] 把输出赋给变量
来源：http://hz.cucudq.cn/gtonwkscca.html

files=$(ls -1)
来源：http://hz.chenlongwang.top/gtozujxgmh.html

[R38] 管道串联
来源：http://hz.cdnleiting.top/gtezkyamun.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jlsjyb.cn/gtjzhodszj.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gtszmnedbg.html

cmd > out.log 2>&1
来源：http://hz.jinghuilouyu.cn/gtxmocqcuf.html

[R40] 追加写日志
来源：http://hz.shanyushiyangtech.top/gtvsmkrmwa.html

echo "log" >> out.log
来源：http://hz.haohaochexian.top/gtkzuxsvmz.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gtnkopzfid.html

cmd >/dev/null 2>&1
来源：http://hz.vqdsnc.cn/gtuowilocb.html

[R42] 输入重定向
来源：http://hz.yvedp.cn/gtpttecfeb.html

wc -l < a.txt
来源：http://hz.iojbl.cn/gtdojqmwds.html

[R43] 按名字查找文件
来源：http://hz.hammf.cn/gtsmodfjki.html

find . -name "*.log" -type f
来源：http://hz.ehwqpu.com/gtjbtcmoth.html

[R44] 按修改时间查找
来源：http://hz.smart0.xyz/gteoshcpwt.html

find . -mtime -7 -type f
来源：http://hz.redwolf501.top/gtvjhwbswe.html

[R45] 批量删除
来源：http://hz.shzxlz.cn/gthcwdtkpq.html

find . -name "*.tmp" -delete
来源：http://hz.hongshengwenyu.top/gtsunthuda.html

[R46] 递归替换文件内容
来源：http://hz.xziqi.cn/gtfzzedtmd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.fengsongda.top/gttzoqgsnl.html

[R47] sed 单行替换
来源：http://hz.cucudq.cn/gtvilyqabh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yueranfly.top/gtfmhbtcex.html

[R48] awk 取指定列
来源：http://hz.nanxuanxn.top/gtccanudin.html

awk '{print $1, $3}' a.txt
来源：http://hz.52xcode.cn/gtxvycnsoq.html

[R49] awk 带条件
来源：http://hz.hnqzz.top/gtethlssgx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxinkj.top/gtbujdqtrn.html

[R50] awk 求和
来源：http://hz.tian-w.cn/gtlfmoffuf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangtech.top/gtbvlnnowg.html

[R51] 排序去重取前几
来源：http://hz.chenlongwang.top/gtdegyiphm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhixingplan.top/gtuiyybqoy.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtbzspmujs.html

wc -l a.txt
来源：http://hz.aibaodan.cn/gtkrhjmfza.html

[R53] 查看文件头与实时尾
来源：http://hz.ivvv.top/gtzbxmlcnl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhiwuduotai.top/gtxvdwdiun.html

[R54] 比较两个文件
来源：http://hz.guannengcc.top/gtufdbmhpk.html

diff a.txt b.txt
来源：http://hz.sxryk.cn/gtwzkfxykr.html

[R55] 压缩与解压
来源：http://hz.chenjidiqi.icu/gtvntilfov.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.aizwys.cn/gtwsaszywm.html

[R56] 远程拷贝
来源：http://hz.yangfankeji.com/gtemoooplp.html

scp file user@host:/path/
来源：http://hz.ppjwa.cn/gtanbmuwov.html

[R57] 远程执行命令
来源：http://hz.redwolf501.top/gtqadnofez.html

ssh user@host 'uptime'
来源：http://hz.feifeiyinyue.top/gtyyhicxjx.html

[R58] 下载文件
来源：http://hz.yj202588.top/gtpxgbvfvy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.bjfxy.top/gtsfpvihsj.html

[R59] 发 POST JSON
来源：http://hz.guowangkeji.top/gtzcwkxmue.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sysykeji.top/gtrjahlcgh.html

[R60] 只看 HTTP 状态码
来源：http://hz.tian-w.cn/gtfgjhnbhj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.feifeiyinyue.top/gtatilmzkn.html

[R61] 磁盘占用
来源：http://hz.jiagoushi.top/gtkfrqpesp.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtaukaelsg.html

[R62] 找最占空间的文件
来源：http://hz.9152youxi.cn/gtezzqhfyt.html

du -ah . | sort -rh | head -10
来源：http://hz.ehwqpu.com/gtjmdxtili.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gtkuneomlw.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtxlucvelm.html

[R64] 结束进程
来源：http://hz.jianghu66.top/gtrvszqlzd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xylfe.cn/gtabfzzzwe.html

[R65] 查看端口占用
来源：http://hz.xziqi.cn/gtuakgegha.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenzaomai.com/gtpsthdpcw.html

[R66] 定时任务
来源：http://hz.yj20258.top/gtxipnwxhd.html

crontab -e;  crontab -l
来源：http://hz.xuanzx.com/gtufjuuplg.html

[R67] 生成随机十六进制串
来源：http://hz.ywan-chungtsiang.top/gtrdcwobim.html

openssl rand -hex 16
来源：http://hz.yj202588.top/gtckljynrv.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gtyxeehwja.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shzxlz.cn/gtedglpinb.html

[R69] 生成随机密码
来源：http://hz.yj20258.top/gtogttvjmi.html

head -c 16 /dev/urandom | base64
来源：http://hz.guowangkeji.top/gtlvsbtpnl.html

[R70] 时间戳与互转
来源：http://hz.ehwqpu.com/gtxumazzwq.html

date +%s;  date -d @1700000000
来源：http://hz.sweek.top/gtdplcwprm.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtzmnkjuik.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhixingplan.top/gtkwguexec.html

[R72] 等待端口就绪
来源：http://hz.tian-w.cn/gtkeyvknai.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gtwxrnhmtq.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtjllufahj.html

split -l 1000 big.log part_
来源：http://hz.smart0.xyz/gtydnqppvq.html

[R74] 批量重命名
来源：http://hz.guowangkeji.top/gtrsifmpxs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gaohongyu789.top/gtramhlovk.html

[R75] 导出环境变量
来源：http://hz.9152youxi.cn/gtcibnttlv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dianchejie.cn/gtnwkbspbw.html

[R76] 使用临时文件
来源：http://hz.52xcode.cn/gtjwmuvcln.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xingfuxueyuan.xyz/gtmmuoxsqe.html

[R77] 读取用户输入
来源：http://hz.hysaishi.cn/gtnrcmnlui.html

read -rp "请输入: " ans
来源：http://hz.xuetiantiany.cn/gtrzjoebyj.html

[R78] 交互式菜单
来源：http://hz.haohaochexian.top/gtcwwsyzsk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.svipenyu.cn/gtgnxvpivr.html

[R79] 解析命令行选项
来源：http://hz.zycfv.cn/gtnwtxxmur.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuxming.cn/gtbzvzluph.html

[R80] 查看脚本执行耗时
来源：http://hz.gzhubu.top/gtaueihrwi.html

time ./run.sh
来源：http://hz.cheryme.top/gtttmtmyyc.html

================================================================================
来源：http://hz.hfpthk.cn/gtafraymug.html

S. C / C++ 专题
来源：http://hz.zhengqikj.top/gtlarhfcjf.html

================================================================================
来源：http://hz.zdqjudy.top/gtwvlsxejo.html

[S01] C：Hello World
来源：http://hz.andypj.xyz/gtcgkxwylz.html

#include <stdio.h>
来源：http://hz.meibo888.top/gtsrihliov.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ivvv.top/gtpulmggyo.html

[S02] C：变量与格式化输出
来源：http://hz.yonumen.top/gthoytoeyg.html

int a = 10; printf("%d\n", a);
来源：http://hz.shangyingyoupin.top/gtbcvdxyxq.html

[S03] C：读入整数
来源：http://hz.zhongyouzk.top/gtygbewbdy.html


<!-- 参考信息 -->