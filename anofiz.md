代发 wailian999

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dyaosqih.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2ozmpkuat.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2cikwkbmg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2dnpwwgfk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cmbelnei.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wqirfwld.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qmdqvrpa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2bhtztkcm.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2abxqaplp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ikllbjza.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2zkdgyyti.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2vqmdcwrc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yrsbhzky.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cijkbtsm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lmyibihk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2iwfceeac.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hnrdkhcz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zivioqaf.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sliuejny.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cokfkxae.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xlfahlgi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ltmjhggo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sskhciee.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nrieueaa.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ylcofmgy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otdmcqnm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2rdgzrhki.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tapqsmyc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2bnzeggaf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zfuzriti.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tfbywvkq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tusdxrdp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2attbqzby.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kpnojjav.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thntzzzx.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rxaqpers.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pccmrkxv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xxrpjfwf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dzgtcytc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpgkemsf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ntnlhssz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckwuxnfv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wyxtpcqd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ennizime.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vxoqrsnp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qqoxiwzn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rzdiexks.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2pyygbsvr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gpuoqhub.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ardpqpxl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tnxuchwe.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2adazeqan.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqjlapme.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2upkigiqp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2izhpnryg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2sdlpgwtg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2onemjpyz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ywdclsrf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gwbsiunc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2frcqqjdp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2gaggekzk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2boajfwtv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ylvggxsv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dmuvdwtm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ohtityft.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2stdziqcu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nhpvdnpi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bvffrybo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yyhpywnu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzhwetgg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bwliqgun.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kndhvvdj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hgdtgtge.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jjngxtix.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yixcqgqp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pelbdmme.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rysoqxlx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2gejjfhes.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nlorxuvl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hwnwbdmh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2htwbkxau.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zowgsods.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iqfdiyvj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jnwixppp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uktivliz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fnniqfca.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jfvxqpwq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yjxobxsb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ybngkzrs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lysuyigv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pmzonjmi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2brrmynmt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2neggdejm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yzjnkhnk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2moudhspr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2arzlivqa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2eorcwimc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2pvmwzqyt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sngsyeek.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xtgwzxcn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wyoszkme.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kvwlcmnn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2raedpelg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hekkfbeh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2mnadondi.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uqrheeli.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2xrfpkanj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wxhwjsid.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edfyvfai.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2qrikzksq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcfjhncv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xnbojayz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2uqrfoiwn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yqqczuwv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2autdkhjw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2bhlsnnjr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gwccqwat.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2flwidxeo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2bzhrlpfr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2iqzbaxap.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2yzllphli.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2afhnpots.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2omjjtukh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2pudiwbbf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2myzqvjmh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rvkfmehx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qnxlzsth.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ubgockvm.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cckbmkdi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2akmblzyr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2smykmolz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kaleakjf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mwnxqmzg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2zwxdiaut.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2itkutmfn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2udhcyyje.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zbrsetty.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2opfucfwr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mlwvtiip.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qsmhozqz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vvycoynn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bcrypdjy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kkhnopev.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ewqjodrs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2svzebwuw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ezawjzxz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qrbuzpgo.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2olesbcjk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2nntwlbry.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mxpxvdob.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2pkoxbgws.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2imhvsqwz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2bdltojsd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2srngmvzi.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uwcilnez.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2tfbfyfza.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2gnmyodvz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2clwnkiza.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hpulevmq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2biryfeem.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mzlzzosi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2drbkntti.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zkbqwxgi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2prucxukz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zjzzllno.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hlftrjdu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xhghjxyc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2evjdhnoc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2pojexrhe.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wwkrfylt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2fnrovmce.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2tkdausze.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2turwfcws.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2feqtixxr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wdgdzvpx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2bvwydgpj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uiyubqay.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2mppzjwzo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2aklyazbp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2rjzubysc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2oldrwebx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2zkjmuiik.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2yglgawvr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fnzblpha.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2thoosqsm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hnpfqobv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2iaaizlre.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2efzwizzd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nimrtyge.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jouhocfw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2duxbegmq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2cfubcydd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2axpdobuv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2gdbheijv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2idgcaiap.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gnybqdit.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ukkwpkfc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2yylramgh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nggadypc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ijsvowie.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qcncnuir.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zsehlcnp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2bgjnwfpk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2oqnvuhhn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2iahpqyte.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ovvnsvmn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2selrzxen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwurmvso.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vzzwyxxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxxjbqbo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2frcxykdh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2gzfuhkru.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cciipylw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ezsupquu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2abyzoqez.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2eplrzgen.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tqjxgwgf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hifckpfm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xvrpwdul.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uwusljwj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2oicgmwug.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cvakwsog.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mstovmxu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2siduygsx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2nnqapbyp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vvxernfy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2auocvwpl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2yuimbagn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2utlhdtgb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2yirzfoyq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jintblzb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ycsfsezt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dpwoqlxu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jexcphqn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2paqjczfg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zrndlzar.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qhfehmxa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rvindwiu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hbfqkvrk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mlouaddi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2owonxonc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2gyrmqwvq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2qmidjstb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ebjlvuhv.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zvggnbbh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mbnoqxah.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kfbipyhc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lnivemlb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2asxinsky.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ewtqqcao.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vhmyfpvr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2jsmowdke.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gspbbodw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nswcrxjb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2lgylbmsd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rmlqinbt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2lcjnyvsq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2sywtkgkj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qdcdrgkb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2jmdlgtsa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2xmytgjuh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rsprbilf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2mpzlatsr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2bttifneq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2fqfkiwjy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2dtpscesu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lltiwetg.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cesobmzj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2fvpzhaoo.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ecvorily.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2igvmgpnk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gepprxfq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2nvwptjaj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2wgqwozqx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rfunbwns.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2spstotar.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2gttrtlhn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbbchmwi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zbwuncts.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2uoqvrjrf.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2fjjvtzhf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2oizjoeue.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hdtdtjzv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fvtyuhlu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2tvxavkfz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2txyqvqtc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lvlfyxfw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nrasuytc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gazoojzt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hqowjynm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lyezqtpm.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2rfotbyhb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2fipgoxbo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2pxepqdlm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2sadculcg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2byyhpyva.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2npozjltn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2warnlvkk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pjixsfpk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2hulpqzbi.html


<!-- 参考信息 -->