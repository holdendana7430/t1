代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gheqymhlv.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gmumqfelw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gnhwuagls.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gtjyclfpd.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gpifyryfp.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gqpmpkyvd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gzdyqaxne.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gjatnvedr.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/ghqceuqcm.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gxjhvlzsf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gyijdktmi.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gzdhuukse.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gzjvpxxvi.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gpajwehgf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gukpgbcbj.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gptjsnrka.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gubyspxof.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gwphhjeit.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gkkosqujw.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/ghtgpypyi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gbxgegsxo.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gdsijpoxs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/glacikrtj.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gpgwenstx.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gqsdxbzjx.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/grcoppkcj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gxbzynuza.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gvbvysbns.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gyimcogtx.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gbioncpmv.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gqzluybkj.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gorwvaqfp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gdqxhwgdx.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gakdhhpvg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/ggiwhpizb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gpghlwnja.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gfpvwgqmt.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/goaxzakzu.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/girejxxkj.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gglpmzgfr.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gkymltkuj.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/ggjbgvhoz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gfwcgfsqd.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gireylpso.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gtcilcsvg.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/genggpkzg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gjrqlpqiz.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/ghewnzytv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gwjduhjvl.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gixzwwhop.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/ghfcclpap.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gfbwnphjx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/ginehqhiq.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gpyhxfgrh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gjghdogwx.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gcscdiajz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gpkaqqfwf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gkorqjnat.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gvcodchgo.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gscbppnxs.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gtavjlohh.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gchxmcsvq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gyuplqivy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gwabqysav.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gjipimmhg.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gzwklsjuk.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gbhukgpma.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gszdlxagw.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gtrklzplx.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gquaeagvr.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gvgltqddk.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/ghoinedqs.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gpaqvaaxr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gndqqcdff.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gzdlgrevg.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/guqinuzkw.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gtkrovqou.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gefzogybq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gtmjjfsoh.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gcfdokkhx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gqjrlwikg.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gtzfikevc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gknjpbhbj.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gcwreajlt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gdlsaycys.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gcbsokpjr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/grbgycxfu.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gzwhoftmj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/grwbftxks.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/grljpsrsa.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqydarxpn.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/ghgzpcrns.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gectifokb.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gnohnuglr.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gsjmwdquz.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gycuoftvz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/ghickilpp.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/glsuycccj.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gmyswugka.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gcddpnkec.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gaoqnzmoz.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gyadtmbvy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gfwftgyrz.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/ggqkpmlln.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gkppyqpzd.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gvyreonnd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gulabilil.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gaqytprky.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gxrpvcxfl.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/goowmovgx.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gsrjugykx.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gfpemkibb.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gvjgmfosf.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gcnaibtvu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/grvzpvozd.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gdnohutzy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gcgsczpue.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gypegvuaa.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gxflshdal.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/glmomfbvm.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gwgvmyfeh.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gasdlcgll.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gggststdf.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gfxpcoery.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gqjsucnsg.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gihdcyhtg.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gnyzwyhqm.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gxmxljlgb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gxkofbtvd.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gcedcjekm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gohtopfeo.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gdofygere.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gpeobreqe.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/geaneajay.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gzgeqzzwb.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gzfrbbgfp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gcrkrzudz.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gwupeotix.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gdogellyx.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gertbfltq.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gvembugyk.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gsxqrqwnx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/ghvzjosqc.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gtxsrstyg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gmvcupsdq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gxwiumvhj.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gdsmnroll.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnkdtarso.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gctxwtvom.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glbqwhyhp.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gldcgalnd.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/ggdmdgjan.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gjpadotor.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gdaretcmd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gycujjurx.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gasslbove.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gmldlmpya.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gyfraujst.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gnneapoov.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gnbarlghk.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gojahuzrx.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gzcgmcgni.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gwfqmqnjo.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gezikbuee.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gzikkoyhg.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gmhffsghb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/ggkgsbjhb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gorauzxwb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gweismnqd.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/glkznxaun.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gjzjxexog.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnoxytsaw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gxujhaaya.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gqktphdqe.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gmacchaas.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gdlkjsamf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gsinesnuk.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gnxlpbbbs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gjmtspsra.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/gsjqbclxl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gjwkwiqey.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gxbzjkifu.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gzrpraudc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gqnkfpydq.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/guwntabhg.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gwzrmahep.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gkjeqyzpb.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gmpswirue.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/guwegaumd.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/guchutrta.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gsyptyyyy.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gdiiydffo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gzlwytkuw.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gnoewwgkb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gndbukeaw.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gbtmdyudk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/ganiqhbwg.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gzzwzlwri.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gunjeuilq.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gkllylvsn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gxvvheoyw.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gbumpmhoh.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gwugrfsoa.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gbgbkublz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/ghbylzmzg.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gluwulonr.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/ghyflklsz.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/geupbalms.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gownefmqb.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gbgebehzg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/ggfmhhrpf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gqoobnccv.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/ghfqkdvrx.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/guakzloap.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gondcmllw.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/gmwtixome.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gydodbacb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gjhqzqrvd.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gnxufnlue.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gyxptygxm.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gkmtgpvat.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/givtwzaog.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gaenehoep.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/geadhxhvf.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/grbbpujkx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gqtilfgzq.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/grzwcyaib.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gcrthvhbb.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gjernslpd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gooihkxgm.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gmahtfjxv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gppmppspv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gtbsnkivm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gqacjyefb.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/ggeosbejf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/gnmmtnveu.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gjfwmhecu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gmnutdrey.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/gmqyalnvj.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gtrhgqtng.sHtML

[S43] C++：智能指针
来源：http://read.share.zdbjq.cn/Article/details/gvoidrkla.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/guiwvtlax.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gzibgmgxe.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gnokherne.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gqytkhwll.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gbghuplte.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gcoaeklen.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gphbmqzjq.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/gikxvlcqy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gzusmdagr.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjcnbltxu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gjztkuatc.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gdgttdgog.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gnpbwkwnr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gxzfklklj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gjtfhhtgc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gdfqudufe.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gpmxsdlka.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/goaxdvntu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gjexwvurj.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gwrjbnzob.sHtML

[S53] C++：移动语义
来源：http://www.blog.hesvh.cn/Article/details/gahuvasoq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gmmkyorkf.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gptxskapl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/glhtsqhoi.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/glpuulckp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gdzryxyta.sHtML

[S56] C++：optional
来源：http://blog.zdbjq.cn/Article/details/gficjbiqh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gkinwjkvr.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gnowupqkl.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gurggmccz.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gcvutdacy.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.hesvh.cn/Article/details/gxpufxlga.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gqzkaupvk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gpefbawox.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gaimsiwyz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gjvhtmela.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdedcdrdj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gqlczhiam.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcwdqtffy.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gzrvnzxwf.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gblwmndvq.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gmsfvknab.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gbztjjyjr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gstadykcr.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gpaygolhb.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhumwsr.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gicbsboaq.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/ghidottak.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/ggldquuge.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gqxfhnmdd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fehbvm.com/Article/details/grunpeonz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gpoyotkpo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gjmoeeqkq.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gobavkael.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gqoshcxpd.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gktcxeamz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/gqyrvnyuv.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gcdjxpyld.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/govgepdpp.sHtML


<!-- 参考信息 -->