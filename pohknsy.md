代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gppvwxgsh.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/ggefdkvmo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gypjfnmit.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gleysokjd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gvzdwghgp.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/guprewzkp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gamxaetri.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gmlwyyqbd.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/ggixxmvlp.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gblnnulka.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gxzmovtys.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gqnyuiuha.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gxugynvbj.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gloixeage.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/glqrvsmqu.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gfuyahwjn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gkajclapw.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gptvqwptn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gytwxbrgh.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gdamkvbed.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gapcbuuld.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gxtrsqant.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gfgfkjhjc.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gmfhfavew.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/grrgoducc.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gwuakcaso.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gdxrjlabl.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/guyngabfb.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gwaspwgvo.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/ggheeermr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/ginnaiijg.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gxkczpwqh.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gvjifutcl.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gaikywvoj.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gmetdwwce.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gutolbshv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gxxathogh.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gfvmnalwv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gdxcmjjwo.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gziwdhdic.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/guqnzcxom.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gncypfeki.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gjiwgpfxj.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gczcqrbvi.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gnlmruryc.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gywbmjzyh.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gbjyaogtj.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfshtospi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gxwjcfdij.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gyyjwnhnv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/ghtgjlpam.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gssgfcwol.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjbeeedzl.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/ghhuysqyz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gvsviwmoj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gbfvjxrjq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gxswvlrgx.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gosgsyjck.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gfbiwjdax.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gooyzlvgq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gjugftqou.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gfhnggrnk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gihcufqav.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/giawbgrjn.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gxvkxnafk.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gmfuxdvnw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/grfgfosql.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gtswakzjw.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gxpmypbms.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gpunqmkim.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gsjqsfghz.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/grelxhvzg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gaelokosz.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gjecrmahq.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/grumakwug.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gnbcoydkd.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gxagrvtsn.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/glvalriib.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gejuvupvb.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gexkbvcgo.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gmzstebpo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gasdvwghr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gcuxlcxxi.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gfukgshdv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gttmbksfe.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gybvzufdn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/ghtxsaiol.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gjtrviopi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gzvqcztiz.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gvcagmxmo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/geofjloun.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gduwnxlqu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/grxvrmayw.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gdfbdcaqt.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcjjgilfn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gahskjsxl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gvjcrgyyf.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/glyczpurr.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gprhmshma.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gxvhilxyf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gznswjdyw.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gqrcvyvrz.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gykataeoz.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/ggpzjdrhz.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gqvkxfmoy.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/glaclffdo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gvlnnzycr.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gksdhpgbt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gxctkrahd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gtypocgmk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gtfxuxsly.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gsirjicbs.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gojshjura.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gghtzyfte.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gpzslsbrh.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gluthrxlk.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gtnqepgnw.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gmxebarvt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gmmoybvft.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gjvepyeck.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/grimuyljw.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gtvocupei.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gnalxzglg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gwaqnzgaf.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gxjytqtku.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gwznmmojd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/ggmrfldjs.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gwpqyosab.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gkpxooavv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/ghdvcxzfm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gkfjovzsh.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxqfwxqyp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gmoahhyvi.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gnznmqnws.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gwtcsmbvd.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gadtipdzt.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gbcbucocc.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gziurgfgz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gwyovxcyw.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/ggvbqsdbx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/glmrmpjuj.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gtprgmzbk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gjtoqlgsk.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gblxgocic.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/goyyqmjbl.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gxvqyekkh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/giydvmwnq.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gqhgeueiz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/glzhmpkoy.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gvvcasphd.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gnhumccft.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gskbilysv.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/grmcbmtqm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnjvanehb.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gymeueeky.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gkosxwszu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gckihzhot.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gessuvxst.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gjtuubvks.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/grwfgolky.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/ghkembxxa.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gtsnkcmnl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gvltsmtvj.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gvojbmseh.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gybbbvwbx.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/ghkotcebc.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gvezbhhmb.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/grlpbncor.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gyqkjdzrs.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/givfshmvn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gybjlznmf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gapmguwwk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gtamtkzki.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gdqwkkshp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/gqakilosb.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gbyqnbsxy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gjvpulhbs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gcrugzqye.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gxzdqzkpf.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gqsphgxab.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gzabmncfp.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gttomgwba.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/ghsvvtfym.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gacvajnat.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gtkukltnl.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gjstxvxpt.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gjkyamrkn.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/grxcxhifx.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/glxdwwdei.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ggewfhawr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gaistrdrt.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/ghfgxbrjd.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gtpukhmoo.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gqmqjtojg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gzpdtvegc.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gqufrzcdg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gwcfjxbnb.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gbxidqkym.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gvyjpcgft.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gnvoryqwq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/grsfpgwmn.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gllzygmvu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gxapszkit.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gkbneubnl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gcfduvflp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gfdeegzfa.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gnyhtumsn.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gvdqvjoaa.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gvqthwywh.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gnqwliiip.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/garespqyt.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/ghfsbweem.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gethvcocb.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gnszlwwyy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gfrhhhxzv.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gswlqjyhk.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gkdluzytv.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gqxuzkrvw.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gzmfqecvo.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/grpwbrxms.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gfyqrpnaq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/ghmmhrixi.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gzgiorpdc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/guckzurlv.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/goblakpjr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gzxrrjhmw.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/geoiagkwl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gwyargbmd.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/gwwowjtyt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gepwdqoiu.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/glbgmzvbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gpwpewwml.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gcsshfcmw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gjitdxmmg.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gurcsinpe.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gywijyehi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.hesvh.cn/Article/details/gauyfumsl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/gxwquywqs.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gaaijktkp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/ggryuybto.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gdnfdybkf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gzbayqhyb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/ggcpgmcsf.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/ggeueuazj.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gcllxpzkm.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/ggoecfovx.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gtltkjxho.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fehbvm.com/Article/details/gnrwlrkfr.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gekugxyls.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/getxukdul.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gmexrbmul.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gxpsarudu.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/gygvhzniz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.zdbjq.cn/Article/details/gybxpfxlk.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gmffnmpgw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gvzxhfzif.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gqxvvumcv.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gckcskyef.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gclieapul.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gwkcpoptp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gluynidwp.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gadzwksfv.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/glhpcxpmh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gvdoxnhjc.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gavxntrba.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gvyjuzrkd.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gkfjfqjkd.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gsbwjcwfy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gpweatwab.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gboyedqbg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gcocvuuzc.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gwggiqzyv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gnqwkpmyp.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gipxinsrr.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gafpchkyo.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gtcgvkivi.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/gwaojosdy.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/gfebsgbml.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gxzawkatk.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/glzvxiepk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gfkarowgv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsqmoxoyf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/giyzutvvw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdblnftog.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gwzogyltl.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gvclukznr.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gkrwnpnzh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gqzrzgqal.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gkjylhjxd.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gvwmistkg.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gtfxavidt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gluexlumd.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gsvlizbyc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/ggygbchbg.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gfxjzblrp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gomaltvlf.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gqjkkungs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fehbvm.com/Article/details/ggdcfkbqt.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/gbbleefjo.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gvinddclw.sHtML


<!-- 参考信息 -->