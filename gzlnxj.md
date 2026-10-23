代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bgllkfce.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3imwjakjm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fcpmucir.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dubdcffw.html

esac
来源：http://www.52xcode.cn/Article/details/gt3osknkqet.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3xxmbcayc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3konsfxsd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qiimdhxz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rdkntknh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3bydowtcc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wmtuntrr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwhvnibb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3izuxzzgw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ssfascsd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3clzabfvm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hlahsteb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3alyhcxsv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vdvsjvvb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jtvfzrbk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zajvumlq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eanmyrqr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zzrogbos.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dqfxaecf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gnzlsoqn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gvvizhxz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3czyhtpkh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3qtwybhfe.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pjdspoaj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3fgdkkgom.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fqbspvhh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3okyebbty.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tcgacmpm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vumzwerk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3elucsbdz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rktpakqc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ftfakjij.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ikkbkhoq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3pubiauuf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vjjivdvi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3omuyxsww.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3zetmtlhc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3urknyqjx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ccjanmdp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qfegoapb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3pjlpklyy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3opzbrafu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rpondlba.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3uydtwjvy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hiiblszm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3uvewxduf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3clgglznp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3corkmowb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ebwyjufs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zalcolkf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nngpybgc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3unsdsbmx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mysstpkt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gqcibcsr.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hsgvrblv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jmegfvzl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rbumeafz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dczhwykl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3coojqyyf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nrksnmac.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yqtfennx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3egzjykzh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ljbcemxi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrhrcozd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3clcayegp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fjsvzkxp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3pgvgtvem.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3pwlqzxtx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xvysjlsc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3mijxrcbl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3csmrtxar.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3trqbpemx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qbbhlkdz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dfgyjkqr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3srzgsjup.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hoqtbyrh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3lkzitjkm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3qphfmsoq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pnludmok.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wxrzskhb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gzzffjvq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3sswxubng.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ewiznpke.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3apyvufkk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xpuzfskk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3selkdkxc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pbpvwmcv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gkvbaydf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ksewwunu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fvcaqpzl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3oyfhvyky.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3etltihxd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gtqhheiz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ngzsecur.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3poomgaig.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dxkoywpj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cwukpnlr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3iejviquo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3cpfjqlzk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3vtjhfgox.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ezbseoba.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yjvftvsv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3pkchtcik.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3kjpxgurr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3iaovfwze.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ezzgkzfd.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pnqrcrtx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3byfpqbha.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3drhrimju.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ozpariad.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3hmxhanqp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hirunnwu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3qelkfhuy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tflqbqho.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hbhgrffd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3xjkamkyc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3tmltikkm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sveatmkr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3drcusjyc.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zcflprig.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3bogbibuy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rzcizujn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3eidaalrw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3msgzfhmc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3zgcikmva.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hwyssnsn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yxfyktta.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3gjjgkyeo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3tmgcunny.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3axgaxamv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3bxaagqiv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ibivcglq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gscnvrct.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pwpsagqm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3swdapdgy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fpscxcsm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3lgzmfqdp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gbqwwyjt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ffonswrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ternkgfp.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bpgpuakf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgfhrjjc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fvdpmhhv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cgshdhfu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3sartwytx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hduknnos.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3lumdhxtm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hlaikkkk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3mbrdwkrp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3epgiwlsi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bjwwjijk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ulmgjkcq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ukpuvfkx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3thsfbqkg.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ooqxrlqy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3glxxvnqx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3pnjpnjwb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3odzuxpde.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3uuuhcdqn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3thtsnaoo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ejrepujr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cyuqifaq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fyfoxmkk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rupeesmj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3aajdhfdl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3kozpfzps.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hscqkjse.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jumvrwmm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mulrknwz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3apccfsug.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3wxteaefc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xojvosnp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3oyoadzqv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uoetbjtl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hsvdrrfm.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cczhfcht.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3zjrcikms.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jffdmrdp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ksuxmvzr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rbqmdlaf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vwpatefb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3bdcaukcq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gbbrxxic.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3dszclsgi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3kghhpait.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3iwmxcunc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3rqcelemy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vucdhpuj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zmutnhlr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ljhxfrnj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3khjhhxuc.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ejplemar.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wymdzleh.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qpsmrbpu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3dqjpvzlh.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qjclsbwu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3sxgzvkiz.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yumhayvd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pqennhot.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ukdxixuz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3kwnismhp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bhcuawvs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qhloowcl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ujzznybl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xdybkhjb.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sozadvcj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3cuivmfwr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ajydsxkl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3dwekdurz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqhzvweg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3ecnctjof.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3fshbcfgk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lqjwyoyy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ydbldneg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3oueccprw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssryvjcc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vrccnzgi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dpsieksc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3rxggjxue.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cytrcxwf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3pszubmrc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bhprcfdq.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bjzbugah.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tlbivyxf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vwwmquax.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ipgbtyci.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ofgnlqlp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zbcmcmzi.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3smcoaisi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3icgfusog.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3twivpkfu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3dipidfrj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qdstrcvq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3whlekpve.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3uqmecqry.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3gtkkjsyy.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hqrxanmh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3dtmkftta.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3aeahaoqd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3glbyebcf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3sgtzwsnd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3ivbhhhwt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqtyfmsk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bxieewma.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3fffqfsmq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojkoxage.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3mcdpchnw.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3ewivmxyj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rarhcrni.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3zvynayuo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xdnusmly.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3xtqllrmf.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3paejbqch.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3zkyahand.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wnlxudyo.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zbvxihdo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ovsmndwa.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3mymcmdje.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3sgitudzs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3surqgcdd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfcxiwak.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3csszlbcr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lcdqrnhu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3zxcgqqdu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3elcsqbxe.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jbejnodj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nhrgqlfp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3srgkmrjf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3uwhknakd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjaguauk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bfyvrqyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abepybbk.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xtfxzazw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ohuoaafj.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ykefdziy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dvqdhjfd.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3emhrfkve.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3saybphmq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3jargezgu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3fcdeqzox.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xmanmyek.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lgrmhtvg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3xalckkyd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3axodiwyp.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mzoxuymz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3qbgmdqrx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ioralhee.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3spwwgada.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3utsrignf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hhmnofpu.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oikfrxaf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3pxeyehje.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3sxmlrftu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3ckcgspob.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bupumcvu.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qzbpxklu.html


<!-- 参考信息 -->