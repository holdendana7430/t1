代发 wailian999

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gqltecndk.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gfqlysatz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/govngjkpm.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gfhefzptb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/guxfvmdvd.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gqwtlcgxs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gkuvmtchn.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/ggaayqkhv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gjodpiced.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gsoqujddv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gcqbpnwoz.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gkkkgaiao.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gsomjojvl.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gxfvkaasy.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/grtzerjea.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/ghqzgmjqd.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gcijbrjqd.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gsihpbvuk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/ghoepmhkt.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gxqljssyb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/ghfyancoe.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gfewmdsep.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gceuugfqx.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/geddpoyrh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/glqysjqmu.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gpjjlfowt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gykigmofj.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gwsdqqzew.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gjqgfqeyx.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gzojjpnnv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gljsnenbv.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gdqgefwjf.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/grznfjtqi.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gjzvoobwj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gwzbygexs.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gxblihgfx.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/garuodvht.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gikkxhnuj.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gsuigkxsc.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gptkxursj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gcmxqzoda.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gnpxlhebk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gmhkgzkbi.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gfcenusbz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gxntfypeu.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gcsffuxww.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gzbgjqvyi.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/glcfuaqqx.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gunsbzivq.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/ggmpxuqir.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/glwqzsjjr.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gkdqbfyyh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gpykctbce.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gehmnqdfy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gsuqsedhk.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gclkscvpt.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/glyosiqaq.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gkxlebpiq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/grrelbsyx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gnnuyvilk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gxxdfgsgq.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gmrotasza.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gorcxnhoz.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gwglkvzcm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gzynmtcex.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/ghhukrvpr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/grgattsop.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/guujqnujs.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/ggtaouedq.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gbzeexsfy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gumvnpplm.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gnshgzrzi.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gdcoutfum.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gcpjkxslo.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gpahfbxdg.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/glgybglxp.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gtadfjtmh.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/ghgvsxsti.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gggykgvho.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gdnmwqmow.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gwgmphdov.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gskbuhiat.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gxozojxhw.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gvfnxints.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gtkuxqzqp.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gglwdzzms.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gzjymcrxh.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/guiffbttd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkeuhnkck.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gndybypmo.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gsrqjhyde.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gnbywhbkf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gyalmcfob.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/ggqcatqya.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/giiyrukvh.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gaevsegtf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/giinqmqsg.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gypcopavx.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/ginfgxvrs.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gbklwzycu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gibazhgbw.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gnvcvukzx.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gsmvcgpzr.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gxggcfczd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/grseosrwi.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gksthrrqe.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gkosusbmt.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gxrdmdgky.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gswlznmkv.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gnmhsgkhk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/grhhnslje.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gujpmcbna.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gzxlgcaej.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gaaizruxk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gqconkvlc.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gxdzohezs.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gttbtaiey.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gzmdegpgy.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gbuxqnitz.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gwnufmwhi.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/guzhjpdqu.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gwgaozbfo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/ggfgddqen.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/grcxmpmic.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gfoeojlwg.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gosxajjgv.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gleqzjjkq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gvueksrvd.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gomfkbhwt.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gdnnwbcbh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/guchnnktu.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gfzqrggwe.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gvsgsdwqt.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gcgjoltkd.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gbczccdmq.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gxijpwqni.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gwmhetvxw.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gigjvteie.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gndilisev.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gtixxaeqr.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gmomgxmjt.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/guutwzbrw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/goprxkqpb.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/ggtilcrmp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gklmztjqw.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gppcfvgfm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gkrwycftk.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gfnlptmwg.sHtML

read -rp "请输入: " ans
来源：http://wap.zdbjq.cn/Article/details/gvpvkgmao.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gswozhfig.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gvcfusbhb.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gspferwap.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gzikiueuu.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gpytpudbz.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gkcycpgyu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxbpeyhvy.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gbpjinbmm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggwmxoqpm.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gksjqdmtc.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gzpakcmax.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gzasorevz.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gopmbyipx.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gynvwkyux.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gewhcdulq.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gxqcyqzso.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gdaxqpehm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gglxtxhmt.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/glyeuvzka.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/geddshtlt.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gxjhsyzhv.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gkdbhhzkc.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gguedwbsf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gagzcqkri.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gksuytuep.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gvdabgtqv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gderkawmi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gzjnlkjls.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gcicwcxoz.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/ghrsgfosc.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/grlamgidq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gxempbzrf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gqpotqrfd.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gpknsjumx.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/ghnyuxplf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/glmjmyhen.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gmlfxnytr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gpswthcwx.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gspmclrua.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gcbrodcfi.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gvphltkun.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gtujqxhtn.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/ggtygonzy.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gklbpsysd.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjtkswmit.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gyylhoxsv.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gdsbwjlri.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gryxdunhp.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gaukvzpqc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/grrvbvcmz.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gitzsmmcs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gmxnmapww.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gdaxxheae.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gemmhamxo.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/ggvhguosg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gdicpsomj.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gapbhgetr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gnteacqhk.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gckelwfva.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gnkzvpwpz.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gmpyxwyga.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/ghwjyazke.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/grynnthbc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gcameboky.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gataivpuu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/guvwomvfh.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/ggwuzwyne.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gkrwavvbc.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gudekvoky.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gfsgeoowu.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gsnvaobqq.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gjswoxwzm.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gcjepgwue.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gdoqgrxrs.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gehefuefn.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gbosfazlu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gozrkohip.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gfuoyfwua.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gqszjripu.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gtpdazsyi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/glemjdeyf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gnmgeleyv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gpiwoangq.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gtkkdqgvg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gjqmfsrvp.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gkruxfpyd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gecoueqcg.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/glohjjizq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gatychiqf.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gqrdtfygn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gbavemueh.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gndrtyugj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gdcuwaskd.sHtML

[S40] C++：查找元素
来源：http://read.share.fehbvm.com/Article/details/gvyicbnrj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/ggxxbtfga.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gxaofhjyd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gilqtcfpg.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gsftpnvab.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gbsfwdsxa.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gvbzrzenb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gjmretoyw.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gqbwojhjh.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gzratqwmr.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gibbpdpfv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/guogmykpf.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gjmkdxsgb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/ggnjsitqa.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gbvgwifvz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gcwkqmvnd.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gkzscmfpq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gmiqxxhbs.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gmuzpkqrn.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gmoncfvsd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gxdzfjsvp.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gcnuqqyfh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gqvheuewi.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gklelxuom.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gubnfrgau.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/guwriprqf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gzzhqcjbc.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gmgxfylsp.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gxgwxunxy.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gpapcmrud.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gglhxsnzl.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gjnescanr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gwlbdglmu.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gudxpjjay.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/giczvnduc.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gnidtkheg.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gfmcgtdyd.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gofvbsekh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gsrewhodd.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gksbbbgnn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gencifxdn.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gpovdcfep.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gquiwecjo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gynntufjk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gwknzaibd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfezxuquc.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/ggscycnrh.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gsuhtmury.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gvreyidhq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gmdggkgsk.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gbzxojqcn.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gfcevbzkn.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gxrdfgexx.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gggekzfdz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/getgyuhpa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gzbuqbvdv.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gpfitnoky.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gkhkefesn.sHtML


<!-- 参考信息 -->