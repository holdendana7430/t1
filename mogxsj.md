代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2kfgdubwq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2duzybosf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tvxwvikw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zgmxgpxo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2wzgewzxo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2pxnkaals.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2czricgbn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2murnxuke.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bmbrhecn.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2gcggwndu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mrblffoj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2gjzbnaws.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2vhcfpusn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2igexoyip.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2maxufovg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ongckdoq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2booqrxek.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yifykniz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ouwuncgr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yqnosliu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wabzwgcm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qlguhoeq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2vkrqffji.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2wejyrcso.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2fpngyswi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kwotcfvj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tfphklnr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bgwotaaa.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bemlvrxz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jujiahoj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2emqmbqlb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wymmkido.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wpgzrwpy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2npddlelv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yyskajus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owmajbpg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lfbjytyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzumschy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jabnvbul.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rgiqnmnj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qcpnflny.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ogckcruu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ttgpqnom.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2uogfvlpt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2pedteqpa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2oospxybd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2vjuaeqke.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2skpdknaz.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xerxnmqh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2etvzxvis.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2apqepgui.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddhuqyuw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ptxowbcy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fcrbinph.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ynnymngq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ocwzbrgt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kmvldkqx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mixzebqi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jqldughg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2zgroxdaj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mwkukkle.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2afvvntkl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2xqmyueem.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zdcdzels.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2cchmnkog.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhtypgvm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qwkvwfug.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jwifghow.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2phgmcvfv.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zekechvz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rriagpyc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sfxeuxvv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2teiqtida.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nlyvtwvb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2srcoixbp.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2xvjoomup.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qgoyatrn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hzvpirgk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2povinnzx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ubkseoee.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ymrhtpyf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dbecgdvz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sufqhvnc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tuktunnm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tqtonkam.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mfwiuwet.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2khysxtdm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2duoczagw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2crszmkpj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2feakltbd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sdvdnfor.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lypkehpk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2bdlxfwst.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2conlrddo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2yprbacxm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2trzdsjoz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zahfzlet.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2pfswghzs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rkyngrtq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hyeuodck.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2iwdzytph.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2adqzvsnc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2myylxbnx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2yzatmghj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2zxfzsxpf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2llirmomn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kxsyrzud.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dnzijpdh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ociosilt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jvoqjqcx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tkgkwxif.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2izqjqsaw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wfyddgbc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zbkyqxek.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2zegovtct.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mulhkemm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2qhtwosnt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2cbxcpfxg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2lqygtifz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lbekxcwr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rwokrmoj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vguxinbb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2fffsipml.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ysargocz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ndkkpkke.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ecrwjafg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ekljlwbv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bklwxqeh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lxceatbv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nlaujzgz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2buyqjsah.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2nqvvboze.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zlkhquai.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tveolshk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wbeznnpd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ebflsxew.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zcbqaypm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zhkmdgkq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ocukjerg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tkkxxykt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bnscylqi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gvkeondm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dvxadhzn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mgmbpshj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fgvjbujv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2cirvtqfz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tqzlqjgo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2soqsaprg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2giyghpbc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tvrkscek.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zifazgnj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2elcwapmq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2httlbogy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hydsmcwv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vifvuale.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jmeegfwp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hrvredue.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hrnmqotz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rynrdjuc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cobalfax.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2cpgfehod.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gcjmcnaq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2raqvkmej.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2aqpeupnq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xjksabmc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lknvptkc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ylbxzclk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rphdfuuh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jekaropw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bskadehm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2zqsvzvva.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wcnvkesq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2cqoojyqq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2chczayys.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zwpraprt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2snolizaa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qkbcclge.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dutknflo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jjaxdkts.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qxuafcop.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2bhquwwjy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2sbmqruly.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xsvetmar.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uqfqrraf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fkcvwhoj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kgyjaekf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ovifawtd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2gdcrwxve.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2zshztphy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2phcswnjk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ymrltsry.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fszrreme.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2gsfzkzbm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ziccdseu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2eeunhhji.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2kevprdxs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wlzjgosc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2labaotqb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2zohwpmms.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ynbkscty.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ycvlannj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ypoysshv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2uhqvzsiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2beohoqtj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ixdfigbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivotsimw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qmlejqfg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2fazxqjwj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tloexsyk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dwxjgggn.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zlokfqdv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hididdhb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hdlvxsed.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2euekwlgw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2drdasvry.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mlbnqlvs.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2buehimcr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ljgczgmn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2qzjqfibp.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2mamrrsdk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2toeniatl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2mittjynb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2irhubcet.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2okoukfpa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xxofutwp.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2znhjvpne.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2qhkiwfaa.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2azzrkika.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2mgmlisge.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxlslcx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tryflllu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2tgvalqfb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pgpafvqw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rudtodgp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ihmdsqpp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2fczggeth.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2yzskszcn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2drkqsaak.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2meocbcap.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2gvbmihmx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2grketcwl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yymyrpml.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2oitaovlv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zlronfqg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2shorstiz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2jgsrtesl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2aifdotcs.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2kcwndwek.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yjquklxh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tbavrrjd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2whwviwmx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2abmbnhok.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2oifvkzco.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2utjdngye.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pozsnqad.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zphwyget.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nofqampb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2ottckscb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2tjqxyjpo.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2yxxpyoqs.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2njmjyrww.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2fcovlyvh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jyamidwd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mesdkhis.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xqetzpke.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2dvnqxazq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tpkbqvbb.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cqcnizch.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lppuglqg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2riemzrtf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ptfbncbg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yipyljcm.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2wyiusjns.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjcimqyt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dgvlzpdy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yndiwmcp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2uwkksnab.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ykgwrdgi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vogumhxm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wutjnmcb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2rzoscsbq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bbiqwiai.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2yoxqkdxk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qptvmyor.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2rmvetlhv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2tuwayqug.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2pacgwdhb.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2hshgdmbr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bhkebnzw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2nyvkjzhs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2mmznnhxa.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hfhhbdhp.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2vmueveym.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qxrchuia.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjaatiev.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2okxuicrx.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wpbtcpih.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zprsuaes.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2aemwvuek.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywujkrqx.html


<!-- 参考信息 -->