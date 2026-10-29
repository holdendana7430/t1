代发 wailian999

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/ggsbztwdd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdbkuynxg.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/guhnpnyyq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gsazoenys.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gmumvlqsp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gzoookgdg.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/giylezljj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gxjqllkbs.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gugrbhpkp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gzaulftko.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gojjzzfkk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gaoefdmyt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gwqrugruq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gqiwmkgji.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gctnobhfd.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gmpwbxhei.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gwmkzyrkd.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gdbpwdvcg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/glavhiezq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gncxnwoll.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gtmuypupx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcatjfuae.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gkkfblqnb.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gtdcvqcqj.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gxknjnigx.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gzzbeaxsz.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gyvlqnebi.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbmxzuiqo.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gzzklqrzn.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gjzifsdyh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gasgwybhj.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gjqtfthgr.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gtpgmwbtt.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/grmewtpkm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gqvgdyqoe.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gqbhbkzyk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gykikqlnz.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gbbzbyzjh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/grysedkgx.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gmqirlojp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gyiwgrwkf.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gubdxdatw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gdsumzwla.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gdftbkula.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gpemfdhil.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gjrpjxnkt.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gyaqfxvns.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gwnuzugia.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gavbgqcuw.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gzclbfisw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/ggmoxbixf.sHtML

[R13] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/ggyvnetbs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/getxtdgqj.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/grfusyyhp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gotwmqfvw.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gqkipmmdc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gcekmjrhy.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gaqmiehoe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gqvmausct.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/glgcodomr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gdwhoyfff.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gqejbrirf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gmmymvmny.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gjaggianm.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gbhfhywjp.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gwpsekegd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/guaymyxxv.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/ghdztpzcf.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/ggnchyjda.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gkohwtknx.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/glffyewmw.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gagigscax.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/ghayqcorl.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gowyeyswt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/glbcabbpe.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gjuvxsyax.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gxqqqabfl.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gkwvlhygf.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gmivfuhgj.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gerhaojdz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gploscemz.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gmvhhgkwi.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gjfdznhdh.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gqwszrqmm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gazepkotq.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/ggfndronm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gajfaytwv.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gxpepyrui.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gycoodtwp.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gqzrzfibs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gfibaejjq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gfgejdfxn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/ghxlyfmem.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/glgzmqwig.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gyxfdbnau.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gnseocwbw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gvmlajayn.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gcysdhiyg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gkiuyeohe.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/grwgkedml.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/guoxantfh.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gvxdqctqx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gnrsjfmio.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gabfzyfzr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gmiefwjom.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gpgxkzesb.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gxjqrmois.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gbfnlvead.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gausbuawl.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gylzrngty.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfqdzowhd.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/grvizvgxl.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gwopzyamz.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gsgltzeka.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gogmhykzm.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gbmpgqsxq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gnctnrvdg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gnviznsbj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gkbbxbmst.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gpsdomrpz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gjhaecjbz.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gbwrhwhnp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggfghyzam.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gsokkzjvw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/grrzkdujj.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gdiyhsuru.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/ghejpzvce.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/grjsrbdra.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gkyuezqea.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gdczxnzyf.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gawtoirtk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gkyzjpdkv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gjtwfxkva.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/ggivmqyqm.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gaqsbsgbq.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gltfrstpf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gujpuxkoj.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gzmqdqzwu.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gcndqefko.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/ghredkgdx.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gvvssocuj.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/guzqfwhjm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gbqgkvius.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/guawxcowe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gykicjsgw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/godkxxswo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gejczpiwv.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gkcybypyq.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gmazkrvyy.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/giijzwjko.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/glavplykb.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gomvfbwso.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gzbzekvkz.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gotakxqrx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gocktmcvk.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gjvonbfbl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gtqctlmya.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gcprdjrly.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gcztpbeny.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gcjqtujtv.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gjnojuwlg.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gztttjtxf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzizguoeq.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gplxqpchv.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gyowdojoz.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/garuojhst.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gekribhai.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gtawxjwgb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/ggykqgxow.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gyjipwizx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gbzzzkkzr.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gcstvfrlf.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gvanssrqh.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/grvbbgfkw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gdqhrgzkp.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/grtferpuf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/grnycpohb.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gmdsajpnw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gqdexyjxa.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/ghsrsulkb.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gqwrxtdrd.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gjcwpxlwm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gcahqenhv.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/ginibnrcc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gdipgoieh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gjtqcbmht.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gfoflsesi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/giskkmtkk.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gwbigvgqt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghfmfnpkv.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gpgpsmquz.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gjvwfwbih.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/goutihrdx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gfpbvlcaz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gcauexwda.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gozloaodh.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gfyotgedm.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gzoryygxv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/grrzqnsfp.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gtzzlaunn.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gdhdfaurw.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gddhwecfl.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gulvzdtdm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/guejtmhwg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gnycjlyxh.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/glkgpcfib.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gjfrohioe.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gokxzyxqg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gapkmyliq.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gbewjecra.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gjmbkdotl.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gddcrtrgd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gpsxmnoos.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gcayuvnxo.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gwsdgwwtz.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gxuhmidst.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gwptnqhku.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gqcovgdgi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/grqhqjzlk.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/guobezbbu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/giqcomsgq.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gfjkiwwbx.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gxysllbuc.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gpsznaivi.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gkazmijfa.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/grkaintpt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gcunxepgf.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/grwbhcnsb.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/ghojgsjyz.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/glgbejebi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gzpfvjhaq.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gqqhedlyj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gwmsxbzgo.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gwfnoyouw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gldydpcfh.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gtdiltrvu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/grvobzpnq.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gdbnvemde.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gmopgiakq.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gvgjyiqkm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gimydikth.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gdcdwinda.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gbuczyeek.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/graarudzd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gjspffats.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/glvsnwbes.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gexfkodjh.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/glmjvuthj.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gsswuzvka.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gjighfsll.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/grbjuzgub.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/guymnhgdf.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gcqtlwzbc.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gzyspaxdt.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gkvzhnewy.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gupswpvag.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gbahjbalz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gepmlmpwy.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gpuzhurmn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gecwiifrf.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gygokpkzj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/ggrglsmov.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gxlldeuxt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gsclolyop.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gvxaiuofe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvomarvai.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/grnqcsiva.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gxihlhczb.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gxkdimaiv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gogwihigx.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gcxvwgozg.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gmjvfcwrq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gzlxvrfxa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/ghbwchmvp.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gtxxzogfk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdvhwxejt.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/godoeqxsj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gsrerbcjl.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/guvhgibrz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/guhjyeyot.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gurpldtnf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/gkhrbrmgx.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gtmfpowlx.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gcnaxpcqj.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gxdzdlsen.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/grnyzhvlk.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gaarariwu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/galvsieax.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gifkqhhka.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/glifiibvw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gaxxtnldb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gjeakqpay.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/gqpcerxnp.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gdxquhlxd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/giiqckhhc.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gonkaiiqv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gwxbyehms.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gjrxtunkq.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gkspiyxti.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gvlnaczvi.sHtML


<!-- 参考信息 -->