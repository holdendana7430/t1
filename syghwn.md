代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hemflotv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xctypglf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xdzxdkwc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2excjaksd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nkjtxfqt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ekgnaouu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2enrkgbvv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mfaxmpqr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jeyzqlwj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2obevveqw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jyhhckkb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2faljrxzo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2idcoejyv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2aimmoeas.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ugoikbca.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ddkqorvv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2nscagcbw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jqacixav.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2xymobqts.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wpevurmi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tcyvblqz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xqrcqsdl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nvtuuurp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hcacbayc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wdyetqut.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2aqbcbdbz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gyisnvdg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lnbebsil.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xjdbmuaw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2kbqrxfrq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xjkpwerh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jykmtzmn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nsgkbvxc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2fsxfcveo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ophwemxm.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2colkgjjp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ikdqvdkf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dxzunyjf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2upsvtsxk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qmngksme.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2anklpetx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kjaxefat.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2jdecnvii.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rgtbthak.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fmafsclg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tsrohjvd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nqggtrqv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jghugnzh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2knvbgcxf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wmjatlhx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wscdvwtf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xyzvpqcz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2teikvkhz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2aiwbbfbm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rjsthazh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2eeelqrmo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2efempgng.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljtprgsb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2iibxllmn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lfvdmahd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2rzvmwwww.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jnvcjxkp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2waujkiob.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ojchuzvf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2oxdkxevm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tiracjzq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wfhagoow.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ohzypalj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2rhiyhrbj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ufqsuovk.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2akkqpqyt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2zpzkxkod.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2oecbiuuh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2vqpyklqr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2orkhcrux.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2pvcmixwq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2axsvxlax.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ymfcrimr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vhcvzffa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwaaxnmm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fntjvyep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahnvujti.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ztthawjh.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ixtsakjl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ofaddqgb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rohflrjq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gahxliys.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2cxngyfkr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2yfpfqjrb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2lwwfrchc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2sovuxpmk.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2oehtrycv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2aemdamyd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2oowcclde.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdcxnsyu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2artqvyhb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mljkkuxt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2iwbrgxek.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2pbmdxbvq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2didmzqxr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2psudepgs.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aisxwkwb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hedlwrbe.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lgchshdn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2nnamdkbw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mttfknff.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2evwewtjv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ujevrivn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2lamfyins.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjfcbmwx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mjlpqhss.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xcnfuonk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hikskbml.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2sdmekzhk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2okolruzz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fcrmzelg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xymafqmf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2arfrthew.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2dopiuvdm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rcuegnli.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jjpszqhb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2adcrtxdr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qvdbrfja.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xxwkikxh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2prbpzlvx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2gziimivy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jdlrozai.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mrhvtjyw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tsyejbof.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bphmflod.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hozeluoz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hwqhddiw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hydzmbxw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vuirtvde.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nwvbzcjt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jxrauaca.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kmlwnels.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hftyoqmo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fbvyvrrh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2jmctnmjd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ilecnvxs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qvipsiqs.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hobieblv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uhhlxdzr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2utrlicvq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uvmdhehg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2nmexwwzm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2knngwwud.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kblilbgq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mjlgbhxd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dqnvgffc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2btykeqxr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ixvclucc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xygyiuri.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2lqbxybjv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rtqjwgan.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2pvejgbop.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bhiqsnig.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ruatabah.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xxrsggaf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqohaxiy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2owqwemur.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wghugkmp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mqujgrrw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2warekdqu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rnclvmjr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gecdyjlh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bcrwppaz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xkyircoi.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tnlgxrkh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xwodnfco.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vjuzhljr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2qszqsidc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2vsffqrpn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pcglfefa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2btnzfuml.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2chqqetqv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vhwhmbtt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gxppfeur.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lwbbaluz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eupjkupg.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2jznbtnve.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dsoednjh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ofwejrve.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wvbfevki.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qsribqgn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rtmoywhq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nbekqchb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2halsvvlu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dcvcywms.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ciiatdip.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bzazidps.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2riuuyskv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kofrmfrw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2okjfiaug.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2woxhdqsf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tlkcmbln.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yusyfief.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bprqmdnx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2axadnlrf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2iwntzzjx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjdusosh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2azgadfmg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2eoilslfe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ljaqjuxt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gypfbdtv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cyfxokcu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kexohnmk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2rufodswl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2apcczptn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bezhwugq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hwrkuzoo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nffkeaaw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gxkahvdd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jmnqkile.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2hgzvyjaz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hckbfyaz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tgxpxruc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hmptrzzq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mdqbjkwc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2unxmnfzy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ezkbgqjj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2glebiwna.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2abeycfoq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2fohuwigl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bqqbwawc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ppejvvhc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qjjgrbkr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kcujpkou.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vdmphpcz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ywcgyxrb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gfwetyrr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ctppslsp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2eccwnmfs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pqxmmxff.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2czmcxrpl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2jhnsfrsx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2vkpgqoow.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lerrzukn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2edecrvsd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2miqycfrf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ijtrkdcf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2stypxfsv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lfjlgkgt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wqznczxq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2nicxrdtm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2uqofxesx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odwvlwsg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2gzvuwxqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmprfxfn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fewmvkbf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zookaata.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wrxgspnk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ogxrunqf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2gpegklbs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ljeatgdv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2udlmpzxf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ovbzdnxp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bwqzarxg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xyrhkhir.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzqweuuf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gsoqdlnm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2uldnlabu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2epnruebj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2sqrjbsqh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xmrtrxuq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2cxtewhbx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2hfqnjrcn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kmsibxus.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uxevcubp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2wfevhefq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ftjyflhb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2stwftuyh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2tjomqprj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2fgcfkiwt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2vrxhzduc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xiyqdgxa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rhahztjd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vxxlhngg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2uztlgyhu.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2youyzyuy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qwjnnprb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pvksahce.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2cknirvng.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rszrdivo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2csguhxko.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2phjfjcrp.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ceunsrnb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lamuyyrd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2oqcfgxwr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qzzqofwf.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2zphnntkw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xawcjphz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2gzzrcdis.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mqienyox.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rljkpzab.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yrfumlwn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2pvoodjix.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wqdebjaz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2yeulvjwa.html


<!-- 参考信息 -->