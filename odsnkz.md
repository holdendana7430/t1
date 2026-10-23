代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3zkqhgfcu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3nbvundvw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3laknwqyd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wnmepzjh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3brhdajnq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3yefgudee.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3idzzkpie.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jftgvrej.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3voteawsg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ljbrangl.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nqsselsb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vduagvrf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3dmsoddtq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cmpiiolo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hhvkhewl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cyemkgjg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3crznuyxa.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bwymgdsr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gnkezgrb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3olmwotkt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3zsykynhv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tagzqove.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3glxiyxtm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nmgozmrv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3jpxslujh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3uyenusgx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ctxqyudg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qpxzheho.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ztuhqmmj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kuacsmxl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rtwbbgqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csykfriz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ggvqjary.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jeinfcpn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xppwwwhn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3dfjsgksr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3vbbywteg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cixbmbou.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wkbitgky.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3uzzjwpzu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3eaxesrgz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3cwpunsmr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ckaivexy.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dnshoflr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3spuljuns.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mihdfysz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mdhjufdj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3qrmpmjxz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ziemzcjf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3guzjsgpq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lpezidht.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ogzkwbed.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ycyqreao.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3djmjfhdr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ywrtzkio.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ktqiwbem.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xtznxolt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3hiwrlxlo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dmxpicxx.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ucdpllmu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3whdsymms.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3adtsxtti.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3xxvqadbz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yglhfzzf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3crdlanlc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3olzkfjru.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tgpepfux.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3enlobikz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vydoeltm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3uilkhdfb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rmxyiauq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mkqzhjxs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eiwwtmzx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3yjdtjvph.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bsbdtkgx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rasqsqhv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwgyoaec.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ynlcyali.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3csrscjxl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mrzsowdp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jrzcemna.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lxprcoaf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwykvkqk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3tnygrzhg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3kwfooxof.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3grcvonbv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xnnrvian.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3robrnspo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3rxdzvqwq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3xfyitwlv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vrdwhbds.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qawvnawi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3pagmgfsc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rsxrilkc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3voutjnsc.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cdbhoiwa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ciszxalm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ygvfbyns.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3znigmoeq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bdqhiokf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jnynxkcb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3fejizyxd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tujsxntc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3uuhsyjjw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3olvgwkat.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nmsyrkre.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pmoeepaf.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3swadqprt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3gvsxsylk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3askksbjw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wwrmfciz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3gzzizdac.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwjtwyjn.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nctevobl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mmyngqow.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3nqcyqvcx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qydyzupg.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bagbhfop.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3moogxwll.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wqmmqwhz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3usisytbe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3byveetay.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tkfjnqya.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rmptoeif.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3wndgrkui.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3sahxxexr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ziwyxhcv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3nutliehu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3mirvsxbl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xggaqwkl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3rhprvmfn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lgpzfafr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ttijzhbz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hmjkyroj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3aspwrwrg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3zphihmax.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3gjotlxma.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kyunffzu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ehfqwkmx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bklmetgy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3eayumkpk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3iyogoaqh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xnuorkig.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jqfhiwaa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3kvbcalxf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jphvyqty.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3foxjrlsk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lbnpebvt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wkpukdtl.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xmeffeni.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3klcrhuij.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vikgwxzz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ixcspaos.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3yaxlcrbi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lilcdpxv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wjwugkvd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3lwbdtngz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ldcsrpuy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3wealcsto.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3wfupjpdv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3gzhtxqdi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gzffuilc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3kchdizod.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vsthckbq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gclcjxnd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ahugneij.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3auwzhtqt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vymljkhe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bujjjhbx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fsbesggb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hntmfnav.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hziqvpyb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bfndbicq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vnyzevpb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ukomzwqa.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tqcqwiom.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gxqihlkz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3syhgiiqt.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3suskudxi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tjbklbhh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rleocjli.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3smxxqzcj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fnzfriwm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ahsgzpzi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3jnpirsvj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3zczulupr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3sqvhrcrc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3rbfarjqf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rwvfvsoa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3raaxdgvc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cnjmicfe.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3tdbylhww.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3jsecrkud.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3qzvohkml.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gowbhkdz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kxldmfpf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ehjlropf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3qwkyrrlt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3aoekldgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxzaivyf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3fenhugbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mzsneyhf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qzvyoija.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3pgcntjvo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jaclrvqe.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ijdclhao.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fodjncnm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xmxdzmpq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3vtkfarku.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hmukmixi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fqkcmkom.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qjqigkdm.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggrljbyf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rdwijjko.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qpqpyiiu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3wtezqhgo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3blfrwxdg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3zhegkfms.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3liiwwsof.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ctnrmuzj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wugllvkc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rbfngoeh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ixcmfiuq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dcnruzje.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3jobuiolu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3ewxdeuma.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mxylkonx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3uzmkxkwi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nnfyyvbc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dfqzdffr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jyqsknmn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3uwhksnmg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3aihqasqr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hoeahvtc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3soahukni.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fynojbyf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oyetytot.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3guarkqxb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nbtgslli.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3usmerkos.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xvlblygf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ixaciijp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3otaxhhlh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3owrtqcfs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wlazemdr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3xphtfprx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3swurtley.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nyznflcm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3tkwqhosd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3heiwihbi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3skzlucch.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mrwxnrcd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hddvzfab.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3wrqikqwd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3yiaqnrsh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qcweqxir.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3xwkhexdg.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3gjvytnvt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3acwyoutp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xwwpwvlq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3ohnpyump.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3kdnrsqpa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3maxosuup.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3sihaeazp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3awcgzohs.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3aslasmta.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3spmlrlnt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yquhbbiq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xqyzhmnj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3txkixcun.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wfnqhhyy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ysabysqu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vffrbswp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hwflzqwq.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3umbtknbe.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3oowbruqx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3szeyflya.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xrfltmlo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3lmpyvjnd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3leknhqsj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3fbvnlysz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dsauzrut.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3aegrtzlg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lbbqedui.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3horewijx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3rhcigemm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3qwfzjojj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ucodewgx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pguqbsnk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3celxbmbv.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3eaawfhce.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3texajoja.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3rjpwuphx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wbjkcfnx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3rembkzns.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3sqyrxchx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dqczoxrj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ivrxiztk.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3wkcrhqik.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3smawgeyd.html


<!-- 参考信息 -->