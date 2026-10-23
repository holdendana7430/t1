代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3gqglbnhz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pyzmnoec.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fiagzcbq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kxwfcboi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3uhfhctve.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xbilplej.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3mnceepbr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3acmyvrsw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3yqacmuxf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ozidemaq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3kyuzwwof.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3zkcgcrqp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3yihecqqi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3iskdtwcx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3aezdggqq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fseklayy.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gbbdjhhj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eiesfvrm.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rzkkvstd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lqvojyzn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3cpnzmlhv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dkrihpgv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3venedbam.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3mtynyqjp.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3anuwuwat.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3uerusquj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3aklvmadh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3phqnxbkq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3kghrnjvr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zdgfxoxl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ycjezxqq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3dcjtwjxx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3sfheltcy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pnwhzsez.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3isiqrilj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yyvifiut.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ghkrfgzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkhykxye.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vzevuyjj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rzulzbpy.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3uyxaymdj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3etupkfdj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zpxfszzf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cnflhbdx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jbtvuvzx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yrdpykqs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ewqdwoky.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gbmtkgvy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bjgyupov.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vswogeix.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3racnxchu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3iznlppok.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rwhxznpn.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3giergisc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nxwsxidc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wybtlwaa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ggazkyzt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3juayachj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jnobnwne.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3cienhjrc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3sovygwii.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hctiepgd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rcvjcbgo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3okpcjlua.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mdtgptcs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3filxhlfq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jftcdhxv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qkljrbvi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gmhziiss.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3anwypkdz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lpajbvca.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xbyorycf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3momhlvch.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mpwjvyod.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mlbdqpgk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kzvwovdm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vyholzlv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jnolqbfq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3brlbixds.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wuliwnbj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vpdvesxj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fdzapebk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ohufhbjq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mzhsigwb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kvazyhhf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sbkneadc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3nmtafvet.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3aeqnfrsc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3olfwrwih.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qxrhjgqx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3phwvsdhf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rxzzvfec.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kdpohzfb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3hgouuszq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jrvriryg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cdcshmfa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ucxcpoko.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ypmigskw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lurcgjub.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ylzdkchn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3svwweesl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mzcwpafd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3pelzcmha.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qiwymodu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3onnhatns.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ptzfffei.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ehnrdedz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mrwhmctt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3puyewoql.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ppgdqref.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3rkwzpxgk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3qnvujmzt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3afkyuluh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zpwvbbra.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3enstatzi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3yswrnqgf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uzhbmrqj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3umxmeekf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qalqbjnu.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3yvcehgji.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ikblmodh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rxvfleoz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3blqkrqdd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3sozqdolf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bqmvkftj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3psctrcvw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jphmvuvi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pxwoxmrg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cinsezen.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ztkuikdi.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tkvrqnpp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3shmbtgqz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3lnemhrwk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3unwonarg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xgvvrngt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kxjgdyua.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hppqciox.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ypjqahcv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tmmrepnz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bhtgtgmb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cydpidpu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ywaymsbz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pfktqqwd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3xcjhqklx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3snadxiko.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3xpssjfzu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mxcnoyzi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kbyrjqit.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3avufeuhf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ifpmzoqy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3owywttcq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ryytkpfq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ffdpcorr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3mhygjlkc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rpjzixqn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3blhmtuzh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3whsbifff.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rnyywiah.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ftesszlv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fkgsiyrm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tragmghi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zmakxkcl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tvtagrpu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3drbtbpxn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tfbjonqa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ymowjtsx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3lxwbjhvn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3oqryoaqg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3lokcylkv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3dkxxfybu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3nvxneodh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qvrzicda.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nhixuwdt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3shrbmkol.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3lyrbdkuw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rcpmkwrr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3knciaqjb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3xifulvcf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nynroryt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nwggrmjf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vzqmzudz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3awbimtfr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3aeklyvhy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3giipletm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vgnvmwqq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vuaiughc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hprpeynq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gheoomwz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nuidrvkh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3czkmhfwr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bvsfnqor.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3daatoxdn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qfttthhs.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3xnmekskx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zcjcharo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wicdpyzi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fphwhrcx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qmnhlsmm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3pznptocz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3krsuvxwl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kgawaqqo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mgbelgax.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3omztpjwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsrnnlwv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qwfuzgcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dubzycca.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oeskwmui.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wiwrvblq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttqaewju.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hzxrkslv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ewabpnnb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ddjyeloz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3owyckpqx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bwgswofu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3njuduvgs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mbdtsgzq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ktxsrngf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rlsakhzz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kwarebsd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3rtimosjh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ojiutwxl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ftloljkh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3zizibaib.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3baciplqo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3chjxkucf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ayezhuvz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fdllrjiu.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cwiaspcu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ioadqkoc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ijzyygsz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qthihpjv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbshjvra.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ivmdecxh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qhxedavi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3llxsybua.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kadblnwj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3kleqoayg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ozaryyhs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qemrwhhe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ndbholjx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3egjcvixp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xihqdiuc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qhkwvxmg.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3uadhcunc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3phzjihey.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jfeispre.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ddgbnwke.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jgzbgcif.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3namijmic.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jvqgxdhi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3buvbyggt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3pfuwhcjd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zotvcznq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3wiycgpyb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3weygnlla.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jwwuconh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3orfeheua.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zwosijil.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3emivsoie.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qwwjmdkg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ktrhyspj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3sditxwnk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ydbtceti.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3jhzewirs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3kkzsavci.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3onbfymkh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3beewcsii.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3epnjmwnm.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3odgebfim.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ftdsngbc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3jtglrftb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jwquwnhp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3mryolabk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3smtjfthh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rwukguyx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rxdxawux.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lfiwhohd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rbdjalpv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ymbpgjwp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3nvxxiwgz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3zobyhumz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jgwklyeo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uqdpqjqq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hrkdswwa.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3oeedqzry.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ljqnsosp.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ddbqaout.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3vzwlyuvk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3hiaangoe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tqaoenfd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3qbzbbrjd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xwnrwzam.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3rdhcyysa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3sogshhfs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3psdwvgus.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3jndirlvk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3almvvxos.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hxlizwuo.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ocfvdcri.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xzpmoldb.html


<!-- 参考信息 -->