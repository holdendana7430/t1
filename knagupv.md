代发 wailian999

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbkusjqkw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwabueco.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkoydikb.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvhmdctb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlaokdic.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gksdxkuzv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gizkvrfci.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gsrkppewz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gwijpkfru.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzxeppwi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcmwpxfw.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiswltyw.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gncclvfcg.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqrsnvbp.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gosyxgfaj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gagxjekhc.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmozurux.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbfnpjys.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxrfvwbe.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gdisjomhy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvlqokry.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuxqsqmx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsewklpdz.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gftuklpxv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gprpazxdh.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjksvxxgy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gptupmzyw.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgugtrfd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gchkktawy.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkctlswj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/giplveveg.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxuagcwv.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/grcghtjrv.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrjdbjpe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijsddhse.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gloqzbxag.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzwiljal.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhvjsbdz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttoxpkts.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gonhzgxji.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfygxxyw.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gaujyzxqm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gknkugkxb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjtxykwp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjacgunvm.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcquqrxoz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gpazxscft.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/glfiztewx.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyovbikn.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqouzvshm.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gscwamgxa.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatwbskem.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gahyguszu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxqhlocz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbknasmr.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzpoqwbav.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfqwqrvc.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbvdaagc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gceekrbst.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsubfopv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gghekmviz.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gbjxbhhyh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopzwsdck.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/grnecfjdf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gqzkasdet.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gyjsjxdzh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gkngfsodx.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyptlrmu.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdwrtpdg.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godbcuxsz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gfusptpcc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhsenfzh.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgzvssmy.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gdtsccwnp.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgzuivzg.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gijoecrfq.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gevdpsckl.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gvblaqlem.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/goopgdyww.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gukmczdxl.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvrybjjm.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuthxffp.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcolnkxh.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkhyapwq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gobhgzmdk.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gzimvobrw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gibafnowu.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgwskhyh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonupvwrf.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/geogfzitx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gffxmhfff.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gkqmejkik.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gduvbxuys.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/guzkgaicv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkewmnlj.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gqhcrwruq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gtrbeecft.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gqehouznw.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gvbbvxzpk.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnkkogoz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzvwzeexy.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwgxsozwq.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqzjbieo.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoljvpkc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gepdkbdxq.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gqbhhibiw.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gsoeuacpl.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlqxqwzk.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gepzrthal.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gspvhlajl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gnszdrgby.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/grnfxlmff.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfjersum.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnfdknnj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gcbomikcu.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfdbxtci.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/geexjumqc.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/girnrqpsa.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/golvumduj.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayequaeg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/guawbbhxk.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gkjbhznla.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gglhwsmuf.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrbdrxbx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gudzcpqmf.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gurrtjwpo.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnbbupxz.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlqxgnfc.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbvwzsbm.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnntyzbtc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gdhidjfna.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnomdaez.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gklaedytf.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/guvrpltsb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/getpcwcpr.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepssrjsx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyujztspj.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdiknchh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzzigxvqo.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gidhdrvma.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gujxdyhfj.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/grmfphikp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/giwiqavcr.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrirtwvj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgnqamyg.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehgaarqy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkumnwsb.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gaxvgmtgk.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/ghjhsmpjv.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/glwqoisrw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnptqprb.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcmtnyve.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcoynkvp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/geijmlukx.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gzzgomxth.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcuqxwtxr.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gvqscofkb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gopzzagyk.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfbzsxawh.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjyrrzfp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgpexdza.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/geoprtvtx.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/groqmavix.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtfovrtt.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/glevhyfrj.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gxzjfcaob.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gdlbzkzzg.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gwycbooyy.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulbgybsy.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/glrqsjxta.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoeutkgv.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/glxecgedh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gihqhmhst.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcqdezxu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlxlssya.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gggxtxupb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/girdehplj.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gjkybxtqi.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjuhgqit.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhxhtkic.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gssfnlnsy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqtnmuar.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/giiuzzdmy.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzbartck.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/geclmzuil.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgbtuaio.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gfgzubalj.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/grnzwoszw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/glndlyvfk.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyqmjiwyt.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gwbqewvwa.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/giaargqve.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwxnrewo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkmsmnsx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gaglultyv.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gmkpickzb.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzjgbydo.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gcuvlfzdb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gljdgbtqu.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gsetvlaqk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbmvvxqd.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbzmyjku.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gawudhqfv.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gsypsgytu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gguevlamk.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwqiggys.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gckilfwzy.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gcvfolrxg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gzxauvnqx.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gsztxaacf.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtyikrau.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/grcidtnts.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuuaugek.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gakyqszke.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gsdqejodq.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdlmrwvcq.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcniztquq.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjnskihrs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlloknkb.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gzjpoldmh.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gdacqhyyx.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gcvnhdqai.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gqwgixayv.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxajyydrs.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gxqrdwdux.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzohkvzne.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/grjarxjfo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gblbkhedr.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gzanjhrug.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbjcviwzw.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gljefvmkv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcgjycnrc.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzjqcizl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gzcncqitq.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gubntewte.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/garubrups.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfickagv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gzpmbzaey.sHtML

[S38] C++：排序
来源：http://3g.fanxiaobao.xyz/Article/details/gdyqwcelo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefawpgjr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsapsagbj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/goelmxunf.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapyfsdqj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gyosofjdt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guxjcvvnd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gswmuilvc.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gkqjtrsrv.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvkqbvkw.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjvlsrln.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gszvxcsbx.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzdpatno.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gesmmgzsb.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gtwuypuxr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/glpunjhyp.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gqugnpinl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gidmwwmdr.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gmdvvbjer.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwpqqiiqh.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gydnuylpv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/geuvirdvr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gwrcurand.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdraicisc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gxyfkqcta.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gssbdbhrd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gdldsewdx.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gsczvfrhw.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkupetmf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsfdtaaq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjuzftmg.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gdftahozq.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzchxodez.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gctyzbjfv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gwwjsxnsp.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojcwnxjx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfroxvpaz.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlupbehi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfncpfpsi.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsodbqcwj.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gjpwzdnqr.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gryymzuuf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygjyngey.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gxfylvtpz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcnxtmwc.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyynmpri.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrofchjb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwiekoph.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgerxzss.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyfjxyocg.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjivxnkf.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjahdiop.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gmenbkngo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyslwrjk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeohipbc.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gtpqztneo.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlchmuyi.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gcdxjziyl.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gqdsxufmh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gbguhxfnv.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gfrrppxqe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gvodtqezl.sHtML


<!-- 参考信息 -->