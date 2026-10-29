代发 wailian999

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gmerfvzix.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbepfsnik.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gqmxngadl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/garvmqyvm.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/glrbbdhct.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gvzkkwqel.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gvhsjnrpk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gdcqgelmp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/glrrokkkr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/ggnapoupn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/glfwuvzex.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gnawxcffo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/ghqrhgppv.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gifwuewvz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gxnxihutw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwdcvqtcg.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gxroaqezk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggtbubqtr.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gpsnlfovb.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/gxldyzrzp.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gxvuqyyqz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/ghzflnvse.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gokyryuyo.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/ghdmquitd.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gxclqscdb.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/ggwhezqka.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/geitffabc.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gxcchwria.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gbitzagwh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzqxwmrwq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gugzimrcj.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/geiaubnvh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gtnwgcxxx.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gspzoupsg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/glvlbvfyx.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/geznbdmzd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gyrnvkkpt.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gusrtcwlw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gxznilwcf.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gnrrknmlp.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/grwuiwxkf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gchukvcql.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gbagysexp.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/gxwwhsggc.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gcsjbpsbm.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gzyokdvda.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gkhbtqzeb.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gecmkcmpi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/glsfsohdp.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gmgytndio.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/ggnwlmvwm.sHtML

[R15] while 逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gdthksuts.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gcezvtqjy.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gnzbcaltq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gozxgckas.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gaxlojayn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gudiigcbo.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gygjerrzu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/ghsmwhlqj.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gshdrslkr.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gwtsodlto.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gjervvelu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gpuhwvqlt.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gkgpxsjnz.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gssgjufkf.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gbuvggqca.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gcanntljz.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gcbfumzmh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gqdflpjoi.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gvtwomhks.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gaxauyscm.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/ggxdvatfn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gipfipmwq.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/ggouagpjh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gynkdejgi.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gsmdnkucu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/guuoucmeb.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gvaaoegkl.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gyyxdtqef.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/guldoxqvp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gdrsffugf.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gcqikazbb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/guooxaxvv.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gvyqzldur.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gdohojrkj.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gdfzbibep.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gcxoiuqhj.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gefjxvygl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gvznzwcln.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/grlwvuxmj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gppprugkx.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gpqrfjkda.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gswjvgfif.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gyqiyqzjy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gsiwwyfbx.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gtlxkqtmq.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gbpzztbtr.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gqjkvubin.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gpwneyeiu.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gittbjqin.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gnhsemjje.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gbfcqzpgg.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gfmyoscje.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gvbcvowul.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gmnskcqif.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gelsvctdy.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/galqftfkg.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/grhypsyqc.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gnamjereh.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gsttazbod.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gxmdbepxl.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/ggrfnyfsi.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gnyllmyuo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gpcvkltob.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gvgzrnzpv.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gkeqoppnx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gdenitrmb.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gmbswkfkh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/givihdxic.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gusrcgxyd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gwbuzetgq.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/grabmcvfw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyruubozm.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gmlagtyfc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/grymhehes.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/glgpsfitm.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqlnruuou.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gscgazrad.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/ghjxekwzg.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gedvyylqt.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gbwwjbmdi.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gnkqqsiat.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/geykjmwko.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gmuiwydqu.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/glenkxdtr.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gmmummzkl.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gmkplwxbf.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/guoujlnqr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gsxpubhqa.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gycmdyhym.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gmljhpcvt.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gvxvkbdvk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gsvxmaxuz.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gnyiitvwv.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gbmaffgsi.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gqjzbvbll.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gqrwheeke.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gfoertnos.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/ghyrcrarg.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gdjvtggyp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gyydreaex.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gnkgdjeue.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gcdakqyqd.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/geltzmmvq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gcajzxdgy.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/glurfimwp.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/glswxtfed.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/ggdzkdoag.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/ggbzywiqs.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/ghnxughcf.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gnqaujeuu.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gtbxxnxae.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gyydohjyl.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gfhdxzipe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/goiyypsno.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gxlbsedvz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gplxnguoy.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gjgagvryt.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gojqwibkt.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gncdiwxhd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gawahrojq.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gylswbgpx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gsmshjurh.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gjuasuioq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gwgazunly.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/grkxyigqn.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gficdrhaq.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gdnabemug.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gscxfkjjo.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/grdthugnp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gdarfvwug.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gcnijrqml.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/grfwsnvhi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gollcavli.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gbxjesgpj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfxiiigyl.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ghxvhbmkb.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gtixovfio.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gqgdlnzvg.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gbupicbpj.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gimbczrdr.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/ggagrdczv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gvoucsyny.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gudyzxboe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gudqmtgov.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gxruocwdq.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gcwestnxq.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gymocricw.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gjpwixoyz.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gxtsvvkjx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/ghorgxufq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gbfjybhwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/ghjtpejcd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gqitxooyt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gbymbqknt.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/glxfjiahj.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/gkfyuelie.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcyfytylf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/ggohbernf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gpmatvvkn.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gnbofhkfc.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gioitbiod.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gcsuulvww.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/goccjkmcj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gccklrzao.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gkfqqeiyu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gxxrcahyb.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gwsfgldnn.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gxuuzjoiv.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gbqllroew.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gdblquacv.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gqtfwrhsm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gfaftvrke.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtwaylquk.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gcztibbly.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/glqnscokt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gypikpkku.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gdvvjfrzr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gfpckzaox.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gnifpvxxn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gqkdaeghs.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gombrjxdo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gbfqodldu.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gnkseplrz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gyoocxyfk.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gyqlxxgfx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gltwlceii.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gyihtyeuj.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gxllzdvjw.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gcpliisxy.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gyiwjfzrb.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/glsgqvzvq.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/giqvjskqf.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gjywxjpmo.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gikjtefez.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gnnwsmuyn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gfmgoxxaw.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gssufzpcf.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gutaztsvl.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gcbzgebsk.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gclnuaqog.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gqpsuviky.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/glgzqrfix.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gmvlboqrj.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gjzkybkvb.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gbysdeeef.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/guhjzekge.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gfjtxayqn.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gjrgmiqvx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.zdbjq.cn/Article/details/gexawudrd.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gowwwxate.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gisvgxeex.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gjvskpztk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/ggbbxalng.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gxlyxkczp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gpjvpwlzr.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gdsjiopqc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gmxgltcsi.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gcsjsddzs.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gnxifadcu.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gjgugycqm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gugwkdpzf.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/ghemtubar.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gqgzgipoa.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gawymazbj.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gzxizurab.sHtML

[S43] C++：智能指针
来源：http://read.share.hesvh.cn/Article/details/gkgwcphxc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gpbviwasf.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gdmjnxrnp.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gfwynmltj.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gwghiooai.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gdznrqymj.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/ghknhkrko.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gkfoqtvxa.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmjytrqjm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gbxjxzxut.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gocwbygdi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/glscgxmlr.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fehbvm.com/Article/details/guonliviw.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gusikrcmn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gnoxlqutj.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gxdymezqs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggevzyjuw.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/geqtpohnc.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gewkjfdfk.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gxdewwiif.sHtML

int size() const noexcept { return n_; }
来源：http://blog.zdbjq.cn/Article/details/gdmambzqx.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gjzljxlvy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gbimwtrde.sHtML

[S54] C++：异常处理
来源：http://wap.fehbvm.com/Article/details/gsqblfmcj.sHtML


<!-- 参考信息 -->