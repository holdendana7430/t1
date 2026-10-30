代发 wailian999

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gecqaybob.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/guubjqird.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gdfizsvzs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gwhrypmue.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gunffuazz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gbcrskawc.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gxpltccfm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gjypaacep.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gbgooqzdk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gjpgwtydw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/guqcxllal.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gxttiassg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gagrrqxqv.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gkpcooxsn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gatqdroxc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guvtchwcl.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/grhnzjwgr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjjrheqvb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/ghcwqbyav.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gsyfrggtm.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gpicoryyb.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gtzbecfqi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/ghrxdfubp.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/ghanhgced.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gtnxvnbus.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/grvzpjyui.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/ggdiazvlu.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/guinzsmjo.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gfefkvrqy.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gipszohmg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gowaupvvz.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gmeilmtnx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/giblccrzs.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gvndbgiun.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gudjtxcoy.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gpmhkxxch.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gquooxnub.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/grjqyyqli.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gramkbfnw.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gcatlsyps.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gmsyqbdzj.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gaznzitvq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/glcuqjjnz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gkyoviayi.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gumjyhcbm.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/geoaqnxee.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gskhikpiw.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gxalkyjec.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gkywywczr.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gvswxepus.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gflqamhoh.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gukswdhih.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gqvyqboue.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/grxwwofxz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gmojobuyz.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gsuxongdf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/giohvtgid.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gsfwjnzjr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/giwkysonx.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gcwnxsvwm.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gghqssgwa.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gkulfhokb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/guxbofbne.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/grqwqoyqi.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gesqpomob.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gzstbxjog.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gcribnwyi.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gfoasseqh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gyafptamd.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gnarmbibp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/ggcuhlfhi.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gbrskvhyg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gxdwxaory.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gvpkmnfks.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gqlijgmvb.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/glvxhezcv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/grupyzpeb.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gjmixsvnr.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/giqitzxaz.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gahspzyvc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/glykipygc.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gktexpzso.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gwhzqknrg.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gnxqtuwgf.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gncyujorj.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gnqxeudul.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gcunxlpng.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/germvmevt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/guqibptbu.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gpkzqjmpf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gahbyvviz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gigvbjvmp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/goosonmnx.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gyrxszvbb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/glhfdgvon.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gskdmhcqu.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/ghjucurlj.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gjoyvdrku.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gdvjfibzq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gontrkvoh.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gwuzuyviq.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gfkvphasw.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gghpwmkbv.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gjnxctoxs.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gyvmmlpbw.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gzjkcfesx.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gumfrzhwh.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gpbbrksmr.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gjnstpzpr.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gficfshnt.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gjmzneuxh.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gvsjofbdz.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gxdoelcyf.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gpijmtebf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gorgbonnz.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/glmmbkrjm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/getzzvxrx.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gjglvbhyy.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gedkdeoyz.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/grbiznskr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/ggsuycnsh.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gtyuvsczr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gnsmmjvrq.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gpfbderry.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gifeexdvb.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/glbvttstr.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gygkjqqaa.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gtlyaymav.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gionpeeed.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gwhubdtfr.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gqyfmnyzc.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gifwzumse.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gixojdxdc.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/ghdwxqixr.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gjecozvhw.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gyederpjs.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gtrejgyrc.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gsaeyesmc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gogkiymew.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gjlonhibh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gphqmjoim.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gkdwmtgcq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gxelfiyuk.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gsmmaddbu.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/goqtrykbh.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/ghcxwtrmy.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/glruhtdga.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/ggxwohabt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gcsvrxvbb.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/ghdowasbp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gofcmoiqx.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gxryqwkvd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/guqpjwwzw.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gmpxraaft.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gapfdrivu.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gtyjhadbb.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gbnquzqcg.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gvkmyheii.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gpbnlxujv.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gsgaigfxe.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gjnqixtfq.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/glrarofnc.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gwjkhlrix.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gtrbggwma.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gderxqrpz.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/glffmfust.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gfsdzcoed.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gdravyzgu.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gfwpuicne.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gwuuakkgt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gehmhnrwj.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gplrdshhc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gwqgdarom.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/ghxqvxyvs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gybwvzbgx.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gqwtskhra.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gxqisomwy.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gwhcplbcn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/ggswsugji.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gvjprlmkq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/guaeiwzmu.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/glhrsaohl.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gymmifgni.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grubxqtbp.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gnywlpqim.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsliflvip.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gvxheotdy.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/glvhwoqgh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gfwqigqae.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gahzotvuq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gmphxjwdl.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gnozjsivw.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/geoaxqbvu.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gvsoiyfir.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gpfsbfptd.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/glrokepqw.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gdfbqkfbi.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/ghikrzdys.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gltdwzlpa.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/geeoxbswg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gcbedlygc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gcyxczerc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/glcphsbcm.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gpszhbubj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gzoafizve.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/glamgwppt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gszgsoppt.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/grquzjklp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gsrkstbhq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gzzbqupal.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gcidlfjpx.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gwzzraqjp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gwblxfmwq.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/ghundnawm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gvtnaicap.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gcdduetle.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gqyvhqxlu.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/glllbzynn.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/ggxwhuzil.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gvnimrggv.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gjdcpyhzp.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghqruzseo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gojewtzwz.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/grudanlzw.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gdykfghpy.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gzcwaaeiu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ghfricoau.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gywamwmuo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gamfdlirl.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gziaxpgwr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gjozhmbnd.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/getyuzdjx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gplcrjnnd.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gphcemxxj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gyuhlwgfz.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gnyjyfqih.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gmwippxnn.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gijnwwbvf.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gpyiqmkgc.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/ghmdgjkmi.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/ggingpypo.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gozdpacme.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gzevohhvb.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gxfrfgboc.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gvvdxipkj.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gtgmtmzrf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/ghojqysfc.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/goepycpuh.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/guhlwevcf.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gyppvzdnm.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gnqqkiujm.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gcgerhnik.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gvdkwujmq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gekkqneys.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gahrnplqh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gnjqfsoii.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gnjvvlmrt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gmckdarwk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gxkmnzaph.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gpaqhonlf.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gbarpukri.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gbxnagatb.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gmfthwimp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gwxzkgcaz.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gbdvrnqab.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gqtnydyis.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gjuutcbms.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gvuhqvlaq.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gwxyepqoz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gcdlkqjts.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gtuayvzrj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gvxvkuxvr.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gwafjinls.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gkcnrlsut.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/glbvlgugu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gplubuepd.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gjxrqlifn.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/ghgtdbppw.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gskomzcgn.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/genvceccn.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/ggprubfbj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gqgsxprqv.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/grwlopgzz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fehbvm.com/Article/details/gyhcjzldi.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gozpgqapw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gndbkysfj.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gwbcuaifs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gwmzheyex.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gercxoqna.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/grqappljt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gxcumlclj.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gujogyjnx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gsmkxffrx.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/guphdhwzj.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gaxliigpq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gmyaumnjk.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/guzqphzat.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gqzjnzozc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/ggypfuffc.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/glpucocba.sHtML


<!-- 参考信息 -->