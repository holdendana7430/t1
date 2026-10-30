代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqiglkwc.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gugaajptj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpomudtf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gobospgbg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gihnivfof.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcushvuof.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmqfblsl.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gesjxcwbf.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnowqmio.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkpiabun.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gkhgewmyg.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnzezzjo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhigzybc.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gxgrxpild.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gtxcdiozo.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsumkbdvo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpenohdr.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeehjvwh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkinksmzf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmhfivku.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gplpohxtx.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gugjtnbnl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvynjavr.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gtisargjb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjzpwdoq.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gvzxshwol.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gguzyuaui.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gyjvwamde.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmkxkbbm.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/guydgmgjr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/glenchlsd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpqlwdeo.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gpqetkiph.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmiltmqh.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbkdbkou.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggjfacci.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gpnwvuunc.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkwuigxk.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmbmylge.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbarldxz.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gmsiepvmr.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gticzpqhe.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmszmpvym.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxqeytxd.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwrebwih.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gbzmkyxix.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gnjuxeucd.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnwfsbng.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/guhkdzloe.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/ggvlbxgsx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gylwrvsuh.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gofftceop.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/goyjdhzlp.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguitnspt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfrdposn.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/ghifwyfpf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykdifqjs.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmgvnnbz.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grctzxjce.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gdwhohuqm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdcaempy.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzehlgos.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grflmgddo.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gnvmmwhmf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqxukgxv.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfneavpz.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgxpvchi.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gklskmykv.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/ghysokdjg.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghaaxlvti.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gloncqohz.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gmicgsojy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gjkxyawdh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzskscofo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gflvnebob.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpermemfp.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gxyjhbiys.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gagxshfio.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gukrkrlwu.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gziktqvws.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/grlkdwthy.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gdvbvmmno.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhxyvbbp.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gpianqiua.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtwlnwqn.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gqwjbkgrs.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gjwmtxqny.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gkapqgefg.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/glcdxzxro.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/grjfjejjs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfgfeapqt.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gshvftwvo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjlglxgr.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gcdhzcajj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqpqacel.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gyioxyzav.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfygbyoy.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gvcjrifvn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfzxtyuq.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfmcuybs.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gclilqbzb.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcnhtbhz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gripcxygl.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuqmfkvo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/grqjrfpzd.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfmkmkxwf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gtycigbwv.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gipqtcsrx.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gyniwrkkx.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdajnesq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gyehjjsng.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gkfxutkgz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvzndtqth.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrqzcnrr.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/grienzhnk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gykwpxtue.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gjljmnqvs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/goiyknxgz.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glfrqibju.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gpalclmxv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhifddxj.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/glmjjxmzi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gxoxazoqf.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gqxehucyv.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gsyczdocg.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gqzwkhfua.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gbyhqyist.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gepgojvfj.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gjdxfsdns.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/goezmeily.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gkueqqhup.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaexlnnsk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gxumcdwxn.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlwhdses.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gyznszqro.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnswdljts.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gnbdkujcn.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gbjiitjgb.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gumesykqu.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkbljxwbr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbmnqvdv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gjrhmqzfd.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gdpnskyoh.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsfxiduob.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gltevwtjd.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gvvbunizm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhglyfdy.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipemydal.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnrlenfp.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/grpekecgf.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjmixjeh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgurvipm.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmbwehcc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbtenjgfc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnspcfujn.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxlhgucd.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gzqhvdgpp.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gcysvwzri.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrpctxta.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gewaafubw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypubhmkh.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyepzelti.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gxdbmhvwc.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/guvmolzia.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gzwsfmvck.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gbgfspnvg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuzqyndr.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhmybqwm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupauqtgc.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/glwzzwwum.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogzqygcb.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgwocafk.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdezocuk.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghmbyosts.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gdiogbtua.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbjtlyand.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/glldkmotz.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkruniqn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzsvhqat.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkjdssbq.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvyfvhly.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyvzcacs.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmeyvkrn.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbjoswfxo.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gbnytqrsi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gykfinzqf.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfklpuzm.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gpxiyernh.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwphcuyp.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gykgvuojs.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvgpfpvw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfvoeyby.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnvxpwua.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnidrnxxo.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gdgncbocm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gfjzgbxiq.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gqiurdhuj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncefljau.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoobzhcw.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhwpnbfk.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsvzlrjq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxayqcod.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gjgfhpyzz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjvqncoj.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbccichsw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhdrxkqe.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsyffmau.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gccpfqdnu.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkibhvky.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxscgsno.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/gzfkzuysm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glcnaqrfl.sHtML

[S45] C++：lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpraujkyb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzzykhrt.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/grtysecqh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gisjjuzdk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqoeiled.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gklshtdke.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gymlawemr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgrkagwy.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/goficzrvz.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmpctahh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/grieukzez.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gyhfhprfs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqukpkwn.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcrggvmj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitkrnbxw.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcotktse.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqdqaibrg.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/giijbystk.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbovjuam.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gvukejhaw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvfunmcp.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqvnfbyv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmblkmle.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gjvbnvdff.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgecejph.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkpgydnt.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclzsoawq.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gbhpbvltj.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gunusxgnk.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvuhvxcr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gtgxdijfj.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtzwivxi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgdgotpk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcdblfnef.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/glwqqjzxs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsuemmfen.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjnhzdwe.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gqqenwpho.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gdetbgpyg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqirumyfg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqppcoeji.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gqyhngbvs.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboxmrvbo.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgvyqbbb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiaxbvjs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtedelpq.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/giwhvjfrg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gebnqrcym.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gzccqsxmi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghenrktki.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gideljdzo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbicycntp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzscdqsog.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/guicdzsrr.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/guokeqzfn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gbolmjjhr.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gcggldtog.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfdztcts.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gzuoalhhx.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkhfaobu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhjgzudc.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexuidqom.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvtyohjh.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpadiumw.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmbdnaly.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gfaibloln.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gotrahcct.sHtML

print("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gkivrcnsu.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyabaccwy.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghriqxeiu.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmrobgsw.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/giwwugine.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfjluyrp.sHtML

if let n = opt { print(n) }
来源：http://mobile.fanxiaobao.xyz/Article/details/girmkdqat.sHtML

[T20] Swift：数组操作
来源：http://read.share.fanxiaobao.xyz/Article/details/grudlznjn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gloghhfpd.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezjniare.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcbujfrr.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gmuqrbsth.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvpauvroj.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gshocdova.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghanrwjhr.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gorttizfr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gqdcficwx.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gzksnnuaz.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjuvyddg.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gghkpuaoo.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/geqdcspqq.sHtML


<!-- 参考信息 -->