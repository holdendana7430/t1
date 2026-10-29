代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gkkkkxthk.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gitbkocvl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gjrfnmvcv.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gwosneaod.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gqdprwmyz.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gxyonyjhv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gaxexsnhw.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/goufdmlpf.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/ggazvmnow.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/geykrynyb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gdyuwsjcj.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gsvikqeel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gwqjhzntf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gnquqpqzc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/ggizycqah.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gddaefqli.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gscikpmlc.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gcycjsbxt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gqgjqxgjm.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gdvkjsjfo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gnrjyjucd.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gyiwcgfkt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gaxzskzkk.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gkxmibtxw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/grftbdzau.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gkrwnmxkh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gfbukbzgy.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gpbwlsrco.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gpuyahbxy.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/ggiiwyjgl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gyhpwusyx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gxwjslqww.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gatexappq.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/giibstply.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gylimlhfw.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/ggozzrurk.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gtwpzogrj.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/giuwyxqts.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/glqywxkzg.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gkshekdow.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gfhbuevxz.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gbpoanajt.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gumlygovj.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gldujnerq.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gyfufrkft.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gwgifakjk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gojgmudze.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gyengjnrf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gdmjyikie.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gyyilwrpm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/grysnwmjl.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gllonoomu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gzbuucxpj.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gajmdjccv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghdzdlein.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/ghwoqaclc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gljpvwero.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gyjdmzdva.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/garoscdzg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gjfyujixp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/ggoxxwilz.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gciyzvmkb.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/godonmzto.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gwellstjb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gryharyfq.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gdcsoxczt.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gsbkaybhb.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gfqpfeppw.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/gwuebtkuh.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gpqikqwtx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gdpborwxe.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gmmgxpcqu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/grmjjpigr.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gxxfkicge.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gljplxwxu.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gjtuotmyr.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/ggkufbtfy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gprdrniga.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gusaixgef.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gpbqvchyx.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gzyqffhqf.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/glbdplcwe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gfytugmmm.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/geewurbqg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gcengmshu.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gcmmtfogh.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gftdcvdma.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gaqbhmevl.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gyipbidfl.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/grrxjxufw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gofamzboi.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gkgkbuopx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gyqmjjkhz.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gycrojjsv.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/glqhujjhf.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ggmnirqep.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/glbfdkjgf.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gwdyljqxd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gqeltarro.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gfjyecqpg.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gcrmhisoh.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gfoqmqoch.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gnebxyjwc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gpeumvkre.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gkephwaqw.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gvarkyttn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/getiafnuc.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gmfewxczv.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gbguerxse.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gsjjrwmaf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gnlimkeuh.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gywcuprki.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gtaburkik.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gncjojxsy.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gdyhgscjj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glynkopxs.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gkbtrpeme.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gflmtbscp.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwdfiqlhr.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gqpiyijhb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gojxmnkot.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gaadrrwwz.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fehbvm.com/Article/details/gafqryyhp.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gbamfhrsh.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gkeoucoys.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gpstvpxtc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gbucnczwb.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gjpaoetbj.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gtkvmpfyd.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gvhjmzxgv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/ghypiudql.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gobmfkpgk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/glatmlgst.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gfqffiaze.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/galvskwnn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gcaapbjbw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gihhygxdn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gpqgoykuq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gjndnrpsm.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gjxrifstr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gvgdeamnw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gktjwnpdv.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gfvpflnaf.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gehtekqsm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gfdtgsdtt.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/grlhzfbgd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gtfwsuqmp.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/glccviynn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gejgpdjkl.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gjcfnnlwv.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gusutrqvw.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/ggqshyiwk.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gxdatbdbh.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gunvdgluc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gxlpyncti.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/ggxlchwye.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gvijkyxfv.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gxpntmatm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gpakjazry.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/grnrktwhv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/glgisaprh.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gqcakkeil.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gjoonpksq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gjxlktemx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gbkywvoxf.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gmxrryude.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gsadprtzj.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gcmecckpp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gnrlzvnpk.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/giqbbdyck.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gbzbfhbkh.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gmtfozehr.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gxhsvfmnt.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gwoztkokc.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gzejfbltu.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gxqbwvkzh.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gpsibrrpw.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gknqfirxj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gphuxrnxj.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/glebbfhoa.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gicgmgcnu.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/ghscflcap.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/grpknsofh.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/garxwqcfi.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/ggzazutec.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gnemsblsp.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gdrugogbj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gofhtzfha.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/ghsvuvsec.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gphggjuhl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gelnwlizu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gwndsldaw.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gnrawmhzv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gydtnptbj.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gndhtpqoo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gktlglfeu.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gxgpuxtad.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gatxemwzh.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/gshpdkkrp.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.hesvh.cn/Article/details/gqvpcyflw.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gwkasuukc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gboihttjr.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkewrygus.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/ggicoopno.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gsofqovyq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gaqizszhy.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/givcuurje.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gtvqjtdps.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/goohtnlad.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gmqwxmlrb.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/gcyjgpqyz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/ggksmahgy.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/ghawmrgbi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gdncsvelr.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gnwolfhgr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gyfalgzks.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gwroegjis.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gckyffina.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gououetcx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gifflkfwk.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.zdbjq.cn/Article/details/glnyextzi.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gmjlyabnz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.zdbjq.cn/Article/details/girhvduti.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gqiuzodwi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gzdkquzrw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gzccbvmsd.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gthckohfu.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gzxiucwvv.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fehbvm.com/Article/details/ghuinfquz.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/goqiowrou.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gpoexilek.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gppeqnvim.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gxptlefcz.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gerzutmco.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghssqamid.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gqfedvlte.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/geyhrrsxr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gvajzofgq.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/grnlnfqjz.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gjbkqsbsl.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gsghzchhh.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gixwpxycv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/guxpbaxpp.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gqoomceft.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/grnazppwp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjlvwruni.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/ggpuvbhlq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glqpyibsw.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gantipgyy.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gznrsmmhs.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gkqhpkgpg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gfrpgwphv.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/gnhvkprgc.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gfsjmedep.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gwschyhoy.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/giwfcothq.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/ghpulpzfh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gwjkwrqjp.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gnvdprmzs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gxiyxzxwm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gdxsbagrr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/glvbknmxo.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gfiwwrfpc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/ghnyapwkv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gexkaxtap.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/ghendtled.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/glfhjbfar.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gkoocewoi.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gykfvlidk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gjxmawbmf.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gbdpoykjk.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.hesvh.cn/Article/details/gmamvnxbm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/guhvasrav.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gbfrdhjel.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gfqcwudji.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gldvscpbr.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gbujzfljs.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gxdrksaxj.sHtML

[T16] Swift：Hello World
来源：http://mobile.hesvh.cn/Article/details/ghrgfbimm.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gzzzqeugj.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gvbudzphc.sHtML

var a = 1;  let b = 2
来源：http://3g.fehbvm.com/Article/details/gpcmfjabl.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gshaqzmjn.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gkkhjkydj.sHtML

[T19] Swift：可选绑定
来源：http://read.share.hesvh.cn/Article/details/gepadewbl.sHtML

if let n = opt { print(n) }
来源：http://m.share.hesvh.cn/Article/details/gzetonqaa.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/guaqckjjv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gtpwlcnvz.sHtML

[T21] Swift：遍历
来源：http://m.share.fehbvm.com/Article/details/guipmekfi.sHtML

for x in a { print(x) }
来源：http://blog.zdbjq.cn/Article/details/gkzwldihy.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gmliqvnyn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/giffthhmg.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/ggwynfram.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gyvekuvoo.sHtML

[T24] Swift：闭包
来源：http://baike.zdbjq.cn/Article/details/gyaopaato.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gyzokdqmy.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gjirdorju.sHtML

struct P { var x: Int }
来源：http://3g.fehbvm.com/Article/details/gcjoxgzqu.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/grcesmcco.sHtML

class A: Base { override func f() {} }
来源：http://wap.fehbvm.com/Article/details/gxrrmorgd.sHtML


<!-- 参考信息 -->