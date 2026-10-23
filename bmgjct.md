代发 wailian999

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bjkfdywu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rbhzbjtq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3inmpfvjk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3rkzdxsrk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3syinodyr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pwouslvs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rueezrxr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ybsbcbgg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3cvfjdorc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3zkxszzkq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qobzfhns.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3nywhnypt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3sqqnmrtr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3veqdehqh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3pqenjplx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nuedklut.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3npoumqhp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ticanuqd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zbiinzlb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vptcuxqa.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vjvkgixz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pzsfhlpo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3laswlvqd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cegsmdee.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3nubwzbic.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lrnpfgjp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vytsfnkc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qavuhrte.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3hpzaglos.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bhxpaxzv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3akvesebu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3yiqfoxzd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wmqtbxiz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3rdejsrvd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifkayhlu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wbazmyqz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gmzzlfbb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uzkxfnwc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hthfeexi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3socrlkib.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3zaijyvmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgcdgdaf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3tznfhqdx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3izucdocb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3mxivnfaq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fkfzlwau.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3xearxsyb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ztagvlca.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wddduhwb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yhocekbc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3yfnbqeor.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pczmcbyw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pqnbdste.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ugovnhkg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfrarmsz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzgsvsri.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bbbfrnra.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3yfjfefrk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wbqeftwi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jvzlxcgq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ulgchqsr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gysxdvaz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dcmmmwhq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3oapaqakk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tlcsafpb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xqserfgd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nlbbnnme.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zpfzixyb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dnxjwdfa.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwakkfqo.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fynkxamr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3clpsvjsv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tnacwcks.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xjeoqbwx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3covrkgrs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfkbwptg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dbptrijl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3zxqyglgo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zqiixoar.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3mkxnsoen.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3mriyjutl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rwvsqqdg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bajyvzwe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wmilrcya.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nqzhoiyj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ywymejis.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3boicgadj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3noftkpwv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wjnbajwp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3eetaksbq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mlwbbvqb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mbardzhf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ppirbyzo.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rxheoqwu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rbkunlqf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3mqwadsts.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3hekcrnug.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3pbjyrxos.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3heiiknrz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3vsphpvmv.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hmwzmlsl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3llrlicpv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3sbwydklu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqgytngh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3cggzgvtn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ecggadzo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hgifwofi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3arfqwbjr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3kgquszyu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3yvltufht.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3okmysqnn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vbvcidal.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hsbyqinj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mddpyatk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ygdomncp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kqlaxajn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pnlukucm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ctrdnjbj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wgcuwhus.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qqvgqbgr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3njbhckmw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wjbxqyge.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gzcwwhek.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3sjjozhju.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lnxxsgbp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nxwlxgfp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3inmizhit.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ncnwgtxg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3appquhop.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3qgkdycyj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lgqlufvt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3zbvdsevc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3qsnvqcti.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3bayzjnps.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wkqkbfyv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xqpxaidq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3hmjuwssw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3squhwrjh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3kzchuqnw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3yzqlodzw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ifspceww.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3falmbkpu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gucsrmwa.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xhvvkimf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3pwwacluc.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gywrsdbw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3knwkhmyf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3elwjgeno.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kthrsbuu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3brrdgmyz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wtmozhzg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3aqgrhysp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jzijqphq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wiaczaol.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ceirjimq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3mnhwtpqp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qdedupgg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3efroecgt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wpclysdm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ddlnsots.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3mbovysef.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xmpzfjmi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3bjtisxes.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jujdomev.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ladxprhl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cfmsiruj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3xnqephcg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3teyinlmd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3kzxefaus.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gvepymvl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jbtsnscu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3xsxasdpi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3mderucpu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bkcqjwmr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xtcpgwpi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3fxvbahbx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gygdvtxr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bscsczdr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jhhwwlow.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3asrocayw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xspdtqlv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3daufesfd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fnfpntvg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3akjjkgmo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3jibeaezl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zhfxqqep.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3dwkjlxse.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iisgbyzc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xwrwzlae.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tsjiwxai.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3plclxxeo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jrqbmtfn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nhsheeki.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lwkehufz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3olhedvno.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tmgfcndq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3chtjkpwd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vfpljqdp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3evuswlyn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dqbklqdv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3moyyozll.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ecesztbl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3dhzfpuxv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3njymuddf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3voeqioml.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gtdzuqvy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zidnyolj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmvflhqa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mfbtskuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqrkwmmy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mihbtrhj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vitykiox.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3cjqyhjnf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vpuleazd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kybehlam.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3feyrffpq.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3erlivgtq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3tsreswbg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gojhawqv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3blyzqkxu.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3medjhpvy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sogekxef.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qwgbtfjx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3quklqhpz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3japfisfa.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3lhymjazt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3rxwulrun.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3mrnnlqmm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3adbxovga.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3niehkcgx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3omirdkts.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tsglksmj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lrojeqjf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mxfurlfp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wmhicspq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzfjdmfl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3melnhgew.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qiskhjfv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gstnwaym.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ndthbcaa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3dotcwuiy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lsgschyo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3wjgtrnlp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bdfnoruq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eihsocjp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jtokvkug.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3moclpzqt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3srkuheml.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3arfbuzfi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rxvhvszt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3swvhwdns.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3qqgyxdrb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ouvmapne.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3cebtkkdk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tjuurhvw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vsmfcqep.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rqtqbobs.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mzrmnjon.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3gkztmlnd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lqxcaczz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fuoymftb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ypjtipyq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xpiugogu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qaljuwma.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3hvubmkbc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3pjwqfmei.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ncnzxwlv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ziexkaev.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tjtcmxdf.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3nyeyrynx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3ymfmmaqn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dinnckfs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xgmqwpem.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3bejgwdrt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vrqwvgsy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xhpuhpfo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3mpdgxurv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndvxlmwi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oezanafu.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ibviekab.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3mgzpamzu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vcoxgpmz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gstsifxr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsdsurcq.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vjivtfke.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bqwfxzct.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3wmztezpi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tvlthdyq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3gguoeiwg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hyuxnfyc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wujhcqss.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3akadfbex.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3itfgizfl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3pwhnrleb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3dtvineex.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wkfotbld.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wxnlecvs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wntsfnbg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwtbxyxe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ymoscmmf.html


<!-- 参考信息 -->