代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gembbwpgy.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gapecepuq.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gdfbjfebi.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gewzlaovi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gcnqdkeof.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/ggpqrsxdi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/ggzticzym.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gtevuthak.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gpohwikzd.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gadlcfnyc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gvxgohtkt.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gsuhiwzdo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/ggbwrxnkj.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gqihfwusd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/glxhtgxjn.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/gkpoxjxis.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gupewscjj.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gekmwvntv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gdrlcjaxp.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gnteswvdp.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gwwlhskag.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gptmumtvd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gnabuwzdo.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gmpabpiyk.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gkpplaeix.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gskxnrzxe.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gxobdsmeg.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gfllixcdt.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gobcnlokg.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gqfipxtai.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gakuyqgie.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gxdxuzrbf.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gfjsvsjhc.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/ggnxstyec.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gxamypcqp.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gnstcneqd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gfeemykdo.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/gwolyjpsj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gsiyhuumn.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gmzaugita.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtwkdaqqm.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gayrrclix.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsgsochas.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gjosddptq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gzujflpvi.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gyleljfik.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gbogjtwfa.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/grzfvbmsw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gvrhetuxt.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gwbthqnnt.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gosnlzube.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gkxnyhkzs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/ggyldsuom.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gbpwjuxhx.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gttjktmww.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gfbzprvsx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gzttcnhhn.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/geejysxje.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gqnwmgzds.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gtixgbyum.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gzcsiwmwd.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gaxzshgvh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gipzgjcmz.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gmasbtzox.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/grtphrfru.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gwxfkjkfr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/ggpigotmg.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gixvjmbte.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/grzqvrtqe.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gewvwtkdb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gepunoaav.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/ggspmvksz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gvwgbvpxk.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gffhimwdq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gpmimsgue.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gvqelxulh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gqlrbjhhz.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/ghuvszfiv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gkcavnapr.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gxsqbeqtd.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gmyjyywyc.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/geswyfxxw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gjopzxpra.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gfqdqhzno.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gizipqynw.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/guzbmlfyh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gohtiexxn.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gydazrzbq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gfcpvblfk.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gkdckicss.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gvuunvsue.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gltewywqc.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gxasiwdxi.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gexlhwvvb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gyvvxgszw.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gagygjryv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gwexpbjuv.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/ghvhfkigp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gjteuhmkv.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gkknmzvjq.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gkvevpedr.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gwpigtcri.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gdsuohnda.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gnfknxpoe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fehbvm.com/Article/details/gfcwwurhf.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gkbnwwlng.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gdqncgghe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtgeurtbq.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gyvgxyzdg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxptctecj.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gmisjtzsh.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/grbbkgode.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxkmjhevq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/ghdbholdm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gquxkcqlb.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/ggsymxubw.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gulwejtjk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gzyxfxcwc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gvckurput.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gfbwbcaci.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gavpwumbf.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gevcunwee.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gxkwslmrr.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/grthcsfju.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gqhaiinpn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gckvisrak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gprqkncku.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gemtgvxpa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gaxmuabzf.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/grpmruryz.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gmjihdtpl.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gumujxmry.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gthzrgyif.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/glrzdalat.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gaxlfbcqo.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gqpowcaya.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gyrarnhha.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gfuexzqio.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/ggtaywkcl.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gioqolwbv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gkckpdywp.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gqgxsygqg.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gayhumxgd.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gklwahvor.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gzcoednhk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gwshpjwxy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gcptfjrdo.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gltzdkewg.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gsxjuxzca.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gsyhisjua.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/grztbwiga.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/grajrdudp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/grtkggucv.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gehexrulr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gjxrbjevx.sHtML

[S22] C：字符串转数字
来源：http://blog.zdbjq.cn/Article/details/gmzzdtrko.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gyeonadtm.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gjqnldaow.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/gixhpjiam.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gvfrysaor.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/guskiexyx.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gabncwahi.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gjnygtkmz.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gyefxbnnm.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/ggbyvljtr.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gromcdnfy.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/guopuicrx.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gonaumblh.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/glzzkaylt.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gxrjhzine.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gqvskqvee.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gbtwqnfkj.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gpairgxon.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gggmvlkev.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gweucvywy.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gbnfhwsmn.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gqxhbphce.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gzvngncmn.sHtML

[S32] C++：字符串
来源：http://3g.zdbjq.cn/Article/details/gighkwvfx.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gydsisjen.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gpzggphjc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gsbdidhyf.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gjmofzftc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/glbiqumqi.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gmllrfara.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gjzmnxkwh.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gnmtvejgb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ggdszfoqg.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gjuatfhtq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gtdfoicho.sHtML

[S38] C++：排序
来源：http://www.m.share.fehbvm.com/Article/details/gtupftaxj.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gyjlsipcf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gyzmgakhl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gkxvngycm.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/gzcycyplz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gyrulotof.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gjcoulezm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gpdburxth.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gqgydqzpr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gpzetomxt.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gnmubnsef.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gollqlrob.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gbzjktqbw.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/golmtkfra.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/geaomeyjf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gbanlyvrn.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gqcqtrdkt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/glqyninfi.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gyuivcxrj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gngenpprz.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/glbaytakl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gbqupfrua.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gkvylrodl.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gccnwapmj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gbfghoriv.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/guwlowgsk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gotxyyraf.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gdxadoxxy.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gmbeixbwb.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gohwksuco.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gyhtaxwyx.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gmdjplqoj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gjmxzhlgk.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gwelglqmh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/glxuxkmbo.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gsktabvse.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gzusarkhk.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gmlqpopwz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gizyrdaea.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/ggzbexnxa.sHtML

constexpr int N = 10;
来源：http://mobile.fehbvm.com/Article/details/gfqybubms.sHtML

[S58] C++：命名空间
来源：http://mobile.fehbvm.com/Article/details/gdkoremve.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gbgtjyouj.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gfanguwsn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gpeyjtgci.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gtfexykua.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gfrwafjnj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfhwmfyhg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/glcumtcqz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaphrgpdx.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/gyvjnwjxw.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkhopyiue.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gruzspcnt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gjuclkiku.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fehbvm.com/Article/details/globtysgh.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gkwtorlts.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gjftspkqh.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/gziylmuks.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gudyatlpr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gysnpkslb.sHtML

[T06] Kotlin：集合映射
来源：http://wap.hesvh.cn/Article/details/gowmccoys.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/ggkdqhfhk.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gsjgjiabt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gbkcerohv.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gsepfwial.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fehbvm.com/Article/details/grbevtimh.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/giwgeqghw.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/gfymxwvvv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gzrzhxzjd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gigzwkvxz.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gvkogjwfu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/ggnqpidop.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gdumwskzt.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gplerhwon.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/giktoyhso.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fehbvm.com/Article/details/ghtkayamg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gbtxaoxfi.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gralbhofu.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gquhttcsr.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gtsfvxxga.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtdnuobdn.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/ganbakaja.sHtML

[T17] Swift：变量与常量
来源：http://baike.hesvh.cn/Article/details/gmwzzxcus.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gsavlwkww.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/guceozfda.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gqnppbabf.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gielbysaj.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gkhfblvpz.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/glpekgldm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.zdbjq.cn/Article/details/gwoytiviu.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gzlpsvvyo.sHtML

for x in a { print(x) }
来源：http://m.share.hesvh.cn/Article/details/gilnxvwta.sHtML

[T22] Swift：字典
来源：http://www.m.share.hesvh.cn/Article/details/gtmcbimwz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.zdbjq.cn/Article/details/gosmebhpq.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gbajghlda.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gewzfwadi.sHtML

[T24] Swift：闭包
来源：http://www.blog.zdbjq.cn/Article/details/gawjocygz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gyogtxmux.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gwszvnfif.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gwcxzvxyk.sHtML

[T26] Swift：类与重写
来源：http://mobile.hesvh.cn/Article/details/gnkxyuixr.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/ghfkfqauz.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gikrjvjbv.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gsbxdneqw.sHtML

[T28] Swift：枚举
来源：http://www.blog.fehbvm.com/Article/details/gpyoefxpa.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/gkhqkqxsm.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/ggowabehe.sHtML

guard let x = opt else { return }
来源：http://www.blog.zdbjq.cn/Article/details/ggbjfuwbd.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gkvpbfqth.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gqxgsgout.sHtML


<!-- 参考信息 -->