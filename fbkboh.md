代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qdccsvrw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2sjzcmwfi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uyomzagq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hiikqnpg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qwrlfptp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ojwuxgtg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2oynrxnlh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kzscycec.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2amokmqoa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uzrbfrpb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rdkdwlmm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kvxrdpcu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2lgfuebyq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wtzqqxqk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2kwbbssaf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2wxbmauli.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2psburpby.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ivgzcvih.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jwnsztvk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xqqpwydq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lcuwlvin.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2awswppuj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ibnzwuhy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2heybpqrq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yygywawn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pthvujpv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2rofrlqqz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2gawavual.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2uiaudlob.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ztteecxm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vpktcikd.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vsbhgonn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pggbhjqq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2jgdxzliv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2rbuilkvp.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2itijahmu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2lkjfrhbz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2caxlsbmt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kkquhxxi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2inmqknxn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bobagtae.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2kxvpkqkr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ghtjjzur.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2tocoodxr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nbpuxrgs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ullsxrcn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rjmsdrcf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zebegcfo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2tbnzhfcr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wvgzcaql.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2msxvqsnb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vdyeuwtg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mgpyfppb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2euhqlrbz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ktvjszcy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nzwnugrm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2yrwgpdwa.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sabmlobs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rkhaekjy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2rfltjrjx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2idcpyxcb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ejxzqjhu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ctpbhxpm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2netvvohk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vvmbsekz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ebxwpcis.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2prdxhuxw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2kibdnopz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tvnirmuw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2yoczlqve.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2iyxbuvdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iedzvsxv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2caxhljcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuhbrjqn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xyxeubsl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jrwgcrvq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2looxwysg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2tmmfvwyd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bqbcdoxz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2iwponrem.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xstfomiq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jyvanhue.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2sgiiwkzn.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pefbkyqk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hibcsziu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2tpusqopd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2aytmgeqo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ztlnxfmm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ttumggzg.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fpqoisrp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wflzwzrg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ezcsnsgl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wmpysifc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2onpqvqco.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2myjbvleo.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2kqpeifnk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2exaahudm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2agdmgtxp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2apqvwjyd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fcfyhabn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2naetglsf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2edgjwwsr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2agzndyan.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2laiklyuo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aswwgisv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2prjyrxoj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ckujatfd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ilhejvyj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2igmfrime.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qedkrtru.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tspupifx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2pnojogfc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qvppuclc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zlucacrm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2yxjjodpf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vvszoewz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jgjlwpzn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2pxenofbt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2shpjsbhk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rixgiwce.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nhsubqjy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2exyqydkw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2xmmchbmn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yrfswgpl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2oxypgtgd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dcoeaatw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mpfxsqhx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2afhoahkq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2pdkpptdf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fmhmghjw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2qlkslfys.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2dwjzwhec.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2xqgrlcka.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2umxcqisx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nwctxmao.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nyfwedyy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2mdmvltih.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gzugqcaq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ljketulw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ibyyuikh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhekwfpa.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2inembtrz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oyphlcka.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ipfftldh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bogpmegi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fekruilt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vdbbfhom.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ktyagaou.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jqgsxsrw.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gykqehkk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ddkkfgod.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2iufovcmn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ztgledti.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jjscqpye.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gnfwmcbb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jbrgfjuh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2byfavegb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2clcscnqv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2algmjhqy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2dglxciun.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jlbtamlr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rxwmnqmi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mmjjjcrh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vxhdtpkv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rfunoaxb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nhklunen.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yhzrxjlt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2keofetwd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lqntqxdm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2wnwtoffe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2aqnfvinx.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2eejzvbmu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kxlbzesy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2fskliinp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ezbsakub.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ernlzykw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2cskwyhiw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2uodrwvyb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2anrjeoab.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2wxfabtwk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nsftfzjp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2zynqrktc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2prgietic.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2iscnrtxy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qmjnkhqr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2oiifijqt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mqvjkpog.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2psgdpyhc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ccxlbczw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2obfpxdkd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sjbqtvug.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ofzgmlkf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2sqfghtpa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zsmqcdig.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2tezbettj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dgqqsfby.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kqkdcopw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wjkyejtu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qkrvyqqr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yoqszycn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2pyjeyyxi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2psxpmxmn.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vosgvmkd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2yujvdubp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2esugzgsz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cjypbzcv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kxwkqfre.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2dnpsnfct.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ikmwbqra.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vrsdwpwq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pbdrmpid.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2vuidlzvw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hpnoorka.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mqieloqn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pquulsby.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rcnwkylw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2egrrouxz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xfiakmpz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2elxzrbpc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cdcqzxhl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ctgvsoeb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jzhlderv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ovcqzvox.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2hpdavood.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2czdgrdkq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ojjlmhlp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2yktedbvl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ziodqohv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2pjwzfvoa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2gkeiahqw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gsflvnqf.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2tgrjeusy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ptdsawru.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lwvaljff.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pmtwooxl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xudmjvvo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2iaxkbrrx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lawxbkmf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2gmkouhxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czydabzy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ftwlfpdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmoewsxt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2edoqwrsr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2scmscujq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2sqhbuihy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dnpnaovd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ctwrzwkm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2kqkabsfw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wcpsnuif.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2bxrztkaf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qapqztth.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xoshjxjl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mtgwlggu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lhgjrcri.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ksuhfeks.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2opxoeirw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2msflshun.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2imxxitol.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2dzquxyoy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2gxdkklkd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nsqzkpce.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2gkqionsw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qmokksuv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kijozhlm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2unzxctcb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tgzijydt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2avvvzonp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2tuzicbfr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xkjcndux.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2eycqsxhw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2aldqreei.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rhycowtb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qtqzesrg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fwnktdax.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lmkdrdjz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rfgenxyh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vjkgktsj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ozqrflyi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2xetmqkhu.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qdkfspye.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2iqomcqhx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qkoouutc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qcuscwtv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2pdsfhjzy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cajgzgie.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2feexezlo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fyqvdoii.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kpodtgcf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2eflksioi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ciokiqnz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2xvcvygzk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2iyrxieht.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lwvpebrh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qxzrhwcz.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bondlnfi.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zgwlakkc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bvgdronk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2iqssvaxe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tjlyyzui.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2quwbhqzs.html


<!-- 参考信息 -->