代发 wailian999

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gmsulgluw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gqjtotlmg.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gbzretxvf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gotgeoksn.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gbqexkipm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gncpnemkb.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gixppxjxt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gvqegswhq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gylcvzqwh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gxncarieq.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gsfszfvqq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gxewycrsf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gvqdgyopl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gmgcpjuaz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geezvdile.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gnpqkydjr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gerwtvgkz.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/guqlwbcuy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/grzoihpbc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaxujsibd.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/grybwwduc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbacwacvc.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gpibxvtnn.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gzqkkflaq.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gtgxzkeba.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/ghszqnedr.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gkelqwfiu.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gionzevxe.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gdtlglttd.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gfqtkfzrt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gbjorllrj.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/ggxlgiwsv.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gwxiunhbg.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/glkqujcsq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gaptbatgn.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/giwhdrbjn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gmszeshct.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gzxhxdlmd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gdhkjgopu.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gumeakgdx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gmrufteng.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gkpjqyuha.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gggwppfuf.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gswmnpdoz.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/glxjhikcg.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gvaeoudbf.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gayspikhb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gppbmhqix.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gxjcyczgs.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gmcuxqoho.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gtrehsuiw.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gnqrlhltd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gfaofwlpb.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gjonxftea.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gowwrboho.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gmbouxyfz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gajmxvawj.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gbanwcjhd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gilfbwrxc.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gzexdurqp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gnqmmuflr.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gyhmzelve.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gvlvzkllt.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gsrjznclu.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gmxrlwtno.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gcnmcwdne.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gvjnzkczs.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gonkpkgvt.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gofjmldyf.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/ghhsmomny.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gqjkvembz.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gpsdlqsyd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gulcvzxdm.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gusblhswp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gjfultjcj.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gvmpyghle.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/grmtqiwat.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gaqlcteaj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/ghkpjbjsk.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gmdmgcbeq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gkpurxefl.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gfduhcolf.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gvgiqhrts.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gbzoqwptg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gybfdneri.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/godpkcaku.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gmsbyedrw.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/giycwdlyx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gaeeawspr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gmkluphhj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gfzsxyvzv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gewxkrgrh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gqdcrcvnj.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrddopa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gqizdxfmm.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/gqjnfqors.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gtaorepma.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gtczsesuz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gkmlkxtxe.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gsvxjfxyt.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gcdqehtus.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gvweozbpa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gwxkndafo.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gpfzpzxka.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gdxxghylu.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gyziniopw.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/ghzooutjp.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/grjhaffzb.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/glzdscfxt.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/grmxnyaai.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gmdmlytjo.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gvoishxrr.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gccbushdm.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gbxspltax.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gwnvfnfup.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gkbvpthtj.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gptigvrqa.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gsqskrrdy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gkfsaumtd.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gyzbgzcxc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gvkzloice.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gfxcilljd.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gsrzigzdd.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/goqrmnwwa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gxfakizfx.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gwddvfnum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gcpfkgntr.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gbobeyhiz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gkniqxvxq.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gnraicabf.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gpxmxyddd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gdgjdqfjb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gwdjkqwyl.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gilzyairc.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gcegvmdbi.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gyzldwusr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gxvcnvvuc.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gdfwkeyzn.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gywntazzk.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gawaolgtp.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gxbxfbspv.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gslyeldae.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gmjnmqkyw.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gmstqxgyx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gvvepskmm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/granepcig.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gzfmkunto.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gowjonbhk.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gyuljltez.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gjpjzuttc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gqqavkdbq.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gesjyulkq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gbmjrifci.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gxludyrls.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gnxqnmnsa.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/giukpxfwn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gvthezaye.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gpjzfmryu.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gmogqtwwz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gizlvlgpv.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gkebvucth.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gwuvzafgv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gkezjbcvw.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gasqtopya.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gtzpfetit.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gcbzovpdw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gladsxqpl.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gzsqayaip.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gngupyars.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gljdkxyik.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gjkefqlgm.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gjeenqjmr.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gjqxhyvjr.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gskwlgsgj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gsnuxnwtp.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gjokzfogc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gugjqfvtx.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gbtwtnled.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gbsgbtceq.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gibqidshh.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/ggjzlekra.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gczqdgmev.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gcxegzqyf.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gaozrgtms.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/godklbyyu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/goshrwspb.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gvqmwwlua.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsihxcikl.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gjhizxxjd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gktpcsoxt.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gzpexrrjr.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gdylkichy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gttfsuega.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gqwyxkyfi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/graazffme.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gleuvvtor.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/grdobcruf.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/glikhknla.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gqugyystn.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gopsjyrsh.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/ghhruyhli.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/ghuhixpxa.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gstredyee.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gfnlhsrss.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gwjzbiwzj.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gvjyhbhcd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gchsayahw.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gcdkwxyns.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gyxzzkpfh.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gxpxpdfxj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gndwtrgpx.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gmgdcetfv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gkegonxmk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gttjjcmxm.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gtuimnvas.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gpzepkwhq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gqgsekzvy.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gejxxdfoz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gzzkdmeyw.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gcwtrlzoa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/guullefuu.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gqjcjriwc.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gyrmhelwb.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/grmpfewwx.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gtgjetxvm.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gawfbbrnm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/ggwxcslsj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/glgfacqit.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gtqazyxss.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/glwzprrtz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/goobdpzrf.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gcjmzsifk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gztcgcyke.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gigdqkhwa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gkubsnesb.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gcyeuguen.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gswfuyevb.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gyvokwiiz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gttqnjovt.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/ghavrgfst.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gabsdqlfw.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gxoxssnde.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gwyvdbtjv.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gxvcotehu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gfyjxzkah.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gmprnagxg.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ghxtfznsz.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gxbukuoyr.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gjzruebyp.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gtnowhfdp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gsspvwftx.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/grgwolmid.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/ggaftuekv.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gipqmvayy.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gdzxkqquw.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gjvpcsjap.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/gsovvonsa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gnqugpjxe.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyoactlho.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gpwkikang.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gpqalvmre.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gwlmwocnt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/geirdjyvp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gupxktgem.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gokyopxro.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gpqplnygp.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gsbwswtyr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/glzqkpuwj.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gdczpekyy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gqxxijxap.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gbuotpwfr.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gwainfywo.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gmawecezi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fehbvm.com/Article/details/gwlbiodhk.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gwnbbngnl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gloflxzpy.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gqcrddwkn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gwvbpqtvt.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.hesvh.cn/Article/details/gvmtmycir.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gqtkqwkxx.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/ggvdiqxnq.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gjxpxmltu.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gbnpczgdc.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gpgnoqzmr.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gbdkznmle.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gnfkojobf.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/ggewukqrc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gqkqnvslu.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gsnnriyei.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/ghprfpbhv.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gwcaqornb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gavdssmiv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gqbcwlcaw.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gomsspdni.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gyqnehrlu.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gvwnsbtif.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gssrioprs.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/ggchrzxhn.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gucwukpfh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/grugxqliw.sHtML


<!-- 参考信息 -->