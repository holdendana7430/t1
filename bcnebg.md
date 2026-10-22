代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vmsmfxte.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2usdmslav.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2nisyewfu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wvvntlpq.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bhriaqma.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jrkstuxj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2aofdcbsc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2altrdmja.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ktjvzzan.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vejhunhp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sjwfkfkp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ibwpmtsm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hrqploax.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nddbntkn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2svyqnaov.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xnylffav.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2sayjbdwm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nsjroext.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qbajfzoj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uwjuttsg.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yrjdjwan.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ohfkipqa.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2lwylyosn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2dtsjadkl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2wfevrmmy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lyeewlip.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ytlwodyg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2vpctxnyu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2yuerxydq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ijvrobof.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2wykskwtv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rqijgttx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fulfzhyx.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vymaansb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kwazlpxq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2dxbblmor.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qjiflgph.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2asaiqrqr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2uhzexbce.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2xskeijzx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rlhtjwhe.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2rypyxmoi.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2dftswejv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2txuezroh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2gqlvrzch.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2apchfyta.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ecpikerl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2yujxxovk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2uduxpnus.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rtebtewx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2izgpipzv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dkkdwnaq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ybzkstus.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bxlitdak.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2arztswrz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2fahxshme.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cubpcwua.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uhdsyrzy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rsatyrvi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxecctzx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jaokqqxm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ubqxgydh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xkcepezc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wgwqackd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2lisasqae.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ioiduwxd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2wauvwcmy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2wsikqytl.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2nhyjtuqr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ntssimmf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2sosvboqa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2plrgmxhx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2btnlqvvn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2uwwigdcw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sqbvabxg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zhvibiho.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tmlwfrzr.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2anpklifz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2dwjarpyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brpscobm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vjvyarla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2varutwbq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zzeiaaum.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ufpiuknr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2njixssgr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qdfppzpl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ulyodndo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2wqbsyinv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hrtlclpi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jlhrqkla.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2kklsqogf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cwuwwdph.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqsamwtd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2mpsrcvhr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wdzewjzu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nqznaifd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zjqurard.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2eppcqurs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2oywlhajc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kerytfil.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pxagoaup.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2cbluqtpm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gutdevql.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2eploshvd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2povtzfds.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jldrkmuz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fzzynwwh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2quknepbp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2diohuuej.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2itgtxeqs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2sjuttyje.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2emrgemkp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ilkckdku.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ifdvjkkj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gmkdrtay.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2liwtwbwm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2tqfcllqg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nbeqszjh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wabeflxd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ajgjwhcq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gjhzyutx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ozyqgkfr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lpdhgifm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ngujcopy.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hznaowwo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2tkdzmhav.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ppchdzsp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rifyfygb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2squwyjxg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2krljimcd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tzcliwqh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hcvzervf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2sppbwqoj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tfgonxav.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jheqampr.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2wynquupf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qdcvijxy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dojdplku.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2cgipbmbu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xuzevtqu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jwwzrguc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ycadziki.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wluzrnrk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gxiojsww.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mqamzwbj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kwnlprnp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hjnzszme.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vwoweyif.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dulmrlbz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2lhxrumgy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pnbusoxm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2swibvzqf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zwbsgvxp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2oihbnsdv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lsdoqzkq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rjgcarun.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vhpslehq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hvkurclj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dgeojxes.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2yqmtjtkb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bpphgjku.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vedtqggv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ztsyezdp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2aebtdyxq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gmtlbayc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2drqrrxel.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jgvdaoyq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2decivnfz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2eqczebfw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2lwoqclzk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jjnaioot.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rzdvthht.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gpycqqjj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ejktvdth.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wzzkgdfv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hoavtkmv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qayzxycb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2vhpxigab.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qwxxygap.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2haqkhvdp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yfrimtzr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dkretgxw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wqdqrcyh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nawwwzpj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2dsxyywge.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2evrmeqhy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sogtykft.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2faoknovh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2yyaipxgs.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vhfcgded.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2qhlplohd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qqujofiq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2spgcmroy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ksdrwkps.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2phtoioyr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2qwzfvpjs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bgkbulsk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2giaetxdq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2sjytylql.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2peeffsuu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2kxoidnkp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rvhptbah.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2edkcjmye.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xgwjeune.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lppvmspx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tjcweoiz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2cwhmfqpd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2maynmkku.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gjhoynhh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pbtevops.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2bqgcqvad.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2dsyqewxw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hoojrluw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2typburnn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wcvulrgc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2tfpgjgcb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2cqxtpixa.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2medwhbdt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2wrtyvtfy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2wvlcufrs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xfokwjrb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qbaoocbx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zumljgyg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fzgbgeep.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dxtkryyy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2avaottvt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ryqyiyka.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2frjuagex.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lwlbudps.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ryczgqop.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ybwoccnd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gjvrqskm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xhmdqpxv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mgxyvwmo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dlakxyxc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xgqyzmfc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ajvxgeak.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2wrwupgrx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xtsueqeq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lewcntbk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2srjifukx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vehmztfx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2mrhfaeah.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xfjczmlh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2osyjqsvz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dsmyjrtv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2mymbaoeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucymnvlq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xrhmnuoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgufrywb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qhugkouz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ybsujczp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yskqqxgi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hankbtem.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yxnpjhva.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bzyrfhdv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ercejnch.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wdztnslf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2badilakt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2eqaqxcxs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2vkjdfhzy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kwpthyvv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bhgxvrkq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nuxpurur.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fmkbwaii.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qhcbykoe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ltykgqhh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2japhpzqt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2hlfabwnh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hnxusfmx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2nirctfis.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pnzfvkae.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2lddwkffz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vqblbshc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eurgqoke.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tqsmmaja.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2twucoxkn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fdjfdsvh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2onjhsxwc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yvrhhqre.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lzxrcnzo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2swayreyj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2kudjdyrh.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yahfkpkg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pgperyaq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ozkvuiqu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2siednbtv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zkirgcrb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ywunlogg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2iocswrco.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2glfocgrf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2hdzgmoek.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ofgxllzr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2yogylwug.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xqsyfupc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ojvmqzyq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tycxewbw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lgmwnzrg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ypibbpvr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2yrwpfyna.html


<!-- 参考信息 -->