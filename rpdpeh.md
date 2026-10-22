代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rgcpipdn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2unjryvkb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2xesjvnal.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2okcpxsnf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kzjkltvt.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vpnjwngp.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lnpctxfo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2cdhcubfm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mrmvprvj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wabgaiuf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ghrcmzup.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bqvlmvaf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kabchwou.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2sqxbrqhg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wqremvvo.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hqvykojc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hjmgghwb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qsvmxnwj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2caxuwkxv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qfurvfeq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rdevovte.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2kufltzln.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2uzgpzoxg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hayvhcnp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2yufkqnmp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mwjsgsbv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ygjsevow.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ksdcpqsr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2iershdrd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2bxoxhgcf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wxspgotc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rcugyzch.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fttzqusi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zufsjzev.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gucimhut.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2vmzeiwtm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qnahwrve.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2kucezvwh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2jbixgxgo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jwkzvdqq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2zanrtmeu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2sooimgdm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2urjjidmt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pvgfhmvl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2juanqxyx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zcqjucte.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2kmhlpqpe.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uzfabrbr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dyfxnkvl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2otpwhoin.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2qrbfbchy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2uzmvsysk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nuonzwjz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2youlnqhz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qvjitomc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rwgkirqy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tvraagkf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mzwhtckc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2gldvozyt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bgsmcaux.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kunkvynw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fnyqhukc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jvbltist.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2vruylojs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2oavgjpyh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2boekypdb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mvadjauy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jseruooy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2eueuucrf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wvhwwoco.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jexoinrl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xagptppc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2cmajcuvg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qkkcwxty.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2oalivtap.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2guykmkyr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zfnsudcb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2msvdonep.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2msdzcybx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2npywmatp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wttupunq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kknbszmo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ijserxix.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2psmzgorv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rciolcmf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2zerpwbsg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gitwgslj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aslejmst.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nlosbwpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnrjtqdk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2yfscljgm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2efatkkbd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2irquytny.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2pfowrgnb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2eotwwcal.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2htcwbdgj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2axkhayrs.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2bgxcihse.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2gvlfpytm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tukiffdw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lxjqpfex.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2jmzqljco.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dmkdsjtx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ssvoovhm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zratqolz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mnknqsgc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2faghmxai.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bqtcbivt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xdqrirdu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qlljqoxt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bbsefueb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2okxgxsdo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vylffcvk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zsgumpfe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2kiscbxfh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xcnyvknf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nsmshrpa.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xhfblqvm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zuzwcfos.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ynupnprf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bllmurxt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hxzpseyn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pbntclxp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kazmuozs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jzpnjgtf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2igadkewx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kgoavfuk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lzhhndel.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2epzynehy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lqnpcowf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jbcfqsrq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lodfmcyp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rvjshjxu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vdxeghkj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sufcwwtn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ibvsrsbn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vdvytpwx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tdhbaavt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ysnmaued.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2gmdezdli.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tgemjhhp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2uvqrsfux.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rpbmcfdt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jvfbuhin.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wketzycm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pyodsevo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ggbsoqie.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2iocvmurs.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wfnacuhg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2arzyalts.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cwhouvwm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2foheqcpr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2adidqjee.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2blfxylta.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mzyynlqa.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uzrlbbhe.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2flkrynmq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rpapoknc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaoubejq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cxlxxaxn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2djigmrfu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dnbmqpea.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2eezpyfnm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wgxfdkpp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2otqknbom.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qhutvoun.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ngqbppoj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ofzsmuwg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dccurwpf.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2uuatyfvd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2pgtaqlhu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2vrfloiof.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mfduprfd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qpcaupqy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rjyfccvg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2odwksmhh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2iuumrvwn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2epekhnum.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ieqyhulm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xdawnfrn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rsmbnozk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nxdkwjtd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2poeflmlp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rgqmhobs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2xomzsaca.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2klnfkreq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2jbmxflfu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zswbynnj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yrruolpq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zowcqakm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2elddgjyl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2frohpptd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2dopmefds.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2irvldnjt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dpykxjze.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2hytwttpd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2dhlhmwzq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lmqjtpmo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rnppiosc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dmwgmbbb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qbyjzhcr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2umjxypge.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jhbtcjyt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2pmejtpst.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2didyxsqy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2qyofgdsx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bayfwrwu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2cksrclhv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dsoyieuf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mebypgtk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2dxzehfme.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fsjcaunt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dtnrncrb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bwstvwkr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qwbxzkxj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rogkqmss.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2unnyooxf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wefdrmlg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dwoemjyw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ydtcinfy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mohdgvto.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dztmumrs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2aktcavui.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2cjjeyakd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qgwjcsbj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jhnqfnhl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ugfzpwhh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qsxvrbgt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mwkhssdx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mqsrnffv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2qebhuout.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2jolegkgo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2onxyjzwn.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dbmrztxo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2jzgdcycc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gpjeuatx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2hsncjdcz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ddtvxtqc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xzbipkcj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mpnfbfuv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2uxorwrvd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2sdaivblq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2kbvtbaak.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qepxkrxw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xezffeps.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fmonilca.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dihkaolt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zitpkzbp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ztfyrper.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xzahkibw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2phyouvzl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ohjvxpdz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2eulyixuk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qgwdzcuo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2oqtfsynq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwmjddba.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ktbwilkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlvgldju.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ulyjsbld.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2msfwwait.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxwojkb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kgkzzhnd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2sjkiiknk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ceggwdpi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ntxnwwxf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jqoibxii.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qfxllvsq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kxmkzzon.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahdbvyba.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rmlgamws.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ofzjeyds.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rpfmvrmj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2rdkdmimy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2qdfpqpzs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2diiluqfi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2rsvoivec.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zipkmbvq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2gswzwgsw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gxvmgbdr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fremsacc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qwemlzsx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rmmtdpdg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2wqjmtjea.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2djbafflq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zknrolde.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2hxjxkldu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2xxiwcqxy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xeniiwtx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2voujgkvx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mrkshhba.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2aywyjgpl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2joawleay.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2knyulwmm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qqaluotn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hoqnypsd.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jcrvfnmi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2mjohmyay.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2wvulxpvp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2axoopiqt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2caelkaww.html


<!-- 参考信息 -->