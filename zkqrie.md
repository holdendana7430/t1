代发 wailian999

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kpkkslsj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gtbtwqon.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2aarmdhpq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ygdwzuid.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cyvpzdce.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2oovyzprv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2oonfhskj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lzpmafnp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2sphrlrnq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xpsrhfsi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vsmjiyxx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bmdexyhv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ndwkikok.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oirokgot.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gkmpgcxj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aaozcpek.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2naafedjl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwiozxeb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gzwxzkiw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2duqigjig.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wiwgnsyt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ichtadeu.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2rjwnpsnl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ayncbjqc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ikmirdsu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rqeqsxbo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rhioivje.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hdtehddh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2allrqxyc.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xpsdxmon.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2atrxbkod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dejxurtv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tqlrflej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqhgvhai.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2nxttfzla.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bilyjfyt.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pmulfqag.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qxxwueuh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yealgjrs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vslvqjzi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ddvpvqkm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vpwctwnp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xhkerwkc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2awiuwbvs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2deuhudik.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2selefuxy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ueglzsnn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uergqyzt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wskjgvun.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ddfhmjyf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mngfzekn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xeucpady.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2trmvidjj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aawolcxp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rqiufzip.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2bfzdepch.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2pxwpngkx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2orhylpvj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wiqlttrp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hpuzjdaz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2prlbscfi.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ofoubbqk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2daudgdjx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2spzagpnp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2foasskwu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2owxibapt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jfshuarx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xkprhcwl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2prwidafv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2eiiglcsk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oxxsiznu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kmywyhne.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2enlnrgas.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2frobwolb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gdafqvfy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jhgqlbya.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hhamrqxe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2uyqwwrrh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kervsakn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xvmzvcij.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2txmqqekz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xkfzlvsi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2hfykaqvh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ksnsfiwc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xqvvuahl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zgypcnqk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tpxjccik.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dkotwiiu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yjfptwmg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gbhhjxgz.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fgztivbq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2njgcsvvx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ofnlbfgn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xyaozolv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zcgwplmr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tgfhrgop.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ibfzquki.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xeglnoai.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2nkdfpach.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qkpgrpfl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bknvyebw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zjuunlxd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhmwnzwf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ydypibxg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2bfzleqga.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2cuygdyxn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ipiqittt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vqrzrgbv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kcccauuy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zafifqid.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dszwxvfp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lpugnrek.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2oabtrjhr.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2jjsjxsup.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2nycousto.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2cdzybiac.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2afqmyzwk.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ozkpvdum.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2fpafrrqq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kjrdzlyp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dtkxcihp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2puhfptxu.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iqebrcyq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2azdgpkzz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ofwkbrca.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wqbjktky.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2nplobplu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ktdqvggy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ylmjwavl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2aabotwxj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jvufpzpn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sddkrlpi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mfiiymjo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rpxlnnng.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bdvlrjdd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zbruyhvj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ughsmpoo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2emthpyke.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kcxenyts.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2komjafzt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nrfrdwin.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ydmsmgkc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kimibmod.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zdjapcpi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nsniofao.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2clzuoqmm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fqavxulq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2xqxthwcf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yswqsbtx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vkuqvadq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gsymaiwt.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ucfwizas.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qzyvumke.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2iuoablim.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dhoheyiz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2shbnzgxr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jcnkfeqo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2aaydwqrx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lvaqsdvr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2aizhrjzk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nogslnpm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fmoqdiif.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gpswutki.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mikysnzr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ktxnvccg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2noigtxkn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2laegytml.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2hgfdxtwl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wcrhuijd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vuqrgaon.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nfregetm.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2chtfxohi.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2cbutqdym.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fiaknrqu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hldpuhzn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2pumwrgml.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2oryfrbye.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kbwbguzc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xpszemkl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oynpemcs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2csbnkrln.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zvtbebns.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mfgoluaf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2zzdrnkct.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qyxrpbui.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ubmteqfa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2nosvmyjl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezbbxnyi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xmkpcaqe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2dysakgua.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qopctymo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ktvnwbqj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2mkxglwoh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ignxlhio.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ezmtnjna.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2wejkugct.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2hwtzigbc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wmlimupt.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2giicrxmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahqsogij.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2logzsbcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wywzpnks.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pscbiuog.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2chdmlvae.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2djytsijx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2aojckhlg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xdcvbcqr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2bbhokbaj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2enaanbiu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2udyesbjr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nosguwhj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2orwlblse.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dexriqhs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2voqbflgr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2yxzllbsm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vdiezgsq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2trkqkxic.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vyaxmzvb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2godpkcpl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2avtdrxhw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pzilkgny.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nqojtjsh.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2lhagzhfy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fklhnqbt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nlyezpsc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vpigpyuh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2lqddtszm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2myazjxwb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qcbmeshp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2iyyvduna.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cthtzqfi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wphnpvih.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ocnvibyg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hlqzlhsx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ytghuvgr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qaramhqz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2vbmkinnx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pppvdpoe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gzzqwtpc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dkbdselp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2wrtcwvwc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2bjreqmrk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vjjwfbfm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2kfqxwuor.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bnebmugs.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2dvayfbxh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2sivvgtuo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2bbakmqxf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dbewcjiq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2vozdrvfe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2dtfzousc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bshbopqg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qggmawvv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bhceozgo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hmouayme.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xazgrebt.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2bwqxuszi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2uhegchrp.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2krrxcsvy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2atlymrow.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qvjehunv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dlwpwhik.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2fxmcbmyo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2fagwkhwh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oyfysqhh.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fjyndyfg.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2rpekggtj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2otwfmkod.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fyzkycqo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqeznmzk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2agmdimjk.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2shhsagye.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2laortjlh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ygwklvge.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xaodcvle.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2skfdgdvr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2dhihxzse.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pxwrkmza.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rwmtnvfw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjrlrouw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2bhfgixca.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ntonutgq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jjgodhrg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qpwtfhzz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2kahoczam.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2avlomvfu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2bofjxhep.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cbmxtxyj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddjnnbcu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wjikbowf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2tkuersgj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2jivuirry.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2saccjkyp.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vfeodusc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xlltxmhe.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2uxjbhrnu.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2oehgjveb.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2sreeherw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2nqvqmuvn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2adeijllz.html


<!-- 参考信息 -->