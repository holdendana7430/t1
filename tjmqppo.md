代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grvbdivqb.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/geclmgtde.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/grugexpbp.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmurbzuo.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gpdmlpvhy.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gqsrqtckz.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gjajmfgxi.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnbkppoc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gofugisvp.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gujrejazx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfzsnuzq.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaqrlfun.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghatnsfye.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlqwxzip.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtdqxdiiu.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdajdcci.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gzasxoaou.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gtqludfix.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/growpkqtz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxfyotca.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvrbyyya.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvwxylea.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceimjgcn.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwvrikpx.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhymqwyi.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjaigajf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gvaiimnwa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmodzcydw.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkswovloo.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/ghwczprbu.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjbwnaje.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrqkcltd.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfopmxzl.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gblwmlyzl.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwimnypko.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvwnfskh.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gctfszdlu.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gloojctrb.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gcxvjhdsg.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqwiwzqa.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/grjmdamnd.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gtfgwabii.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/geergyfpt.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghztggjqd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagnanppb.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gslgjstzh.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnrbpols.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcukmehj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/grcnmovjv.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/geckerbul.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gdvhrbcxx.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/goqrepdxe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfbnohjf.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gtyhxxrnp.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geewnrhct.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gqysjhaph.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmeujcuj.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gahajniex.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaiddffw.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gggqvgglz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gpnqctsxu.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiyocabb.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gyujmdtzs.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbhhodyg.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrkwkxho.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjsrrhij.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gclyasowl.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gllpttotd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ggljegdih.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucludzvp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/giezfgmdy.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsavqgpvx.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkssneuo.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgfxqebn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gervqzasn.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwwzghgl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkrlwpnp.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gymetrckj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwblafowl.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gifqxnmqw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gxktxwusq.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gswxasbsf.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gwgwnzjtj.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/ghgeonafw.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggihhtiba.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/guxtoqqmy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeqdufnh.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gqododaeo.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gicldvcig.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjzmexbl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gzswrispk.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqrqoruo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gfmheakzm.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/guaqubdhb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnusxocer.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/goqufmtsz.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmaivsim.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcpwlglq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gstvpeoxw.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gprmwfuwh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/grrxjkggo.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzffhmqkf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/grzqdnglt.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gagbhctes.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gezznyefs.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gncwnbtmq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckokkuiq.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdfzqtvd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynawgwde.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyulylev.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gegkneroz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geuhqvpoj.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gwxkjmdxo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garchkmpe.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbuyqcdtm.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/ggrcaleku.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxpqpqco.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gjisaldqw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlmiucki.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gmopxwfcg.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/ghtatgcbs.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/giovszfcb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gdsywerhd.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gilkvvlko.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gekceesvx.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvdfyrjw.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsycvxipk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlicujty.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gompcsbbu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpyxabwl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/ghmapsyjp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpogevmkf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gdsvxqypv.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gyzrltkrr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvnvsjjz.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqokrpxhm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gewtiakbm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gobgxlnvq.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gcffoxuku.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guqlxgldx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysonzihe.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gfuefbwse.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gjlfpgmeg.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gmchdwntr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/geiyrgrgg.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gngfezbxb.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwcjobrx.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtmezlnb.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpemukdqk.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gfvuxxoui.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/guqtgtark.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gsmdnltif.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlhshvti.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzdhbeoa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gzbswfcdq.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglcmfpzv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gtuxoktot.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndxbipws.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gqhmfzpxc.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuibluwl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozheurmf.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahlmrgpm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbncrtvtj.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsxoimin.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grssnbszd.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gxxmsoefu.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gdivvdatk.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaqqbzie.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gigybhusb.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gmoxvsoex.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/godebholt.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmwvwwgfe.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbukotxm.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guqlroryy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgmbnoob.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttvhvblk.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/guiqvtauq.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzkeyebw.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/grufeyjou.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnygxcpuu.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqzokuzg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcirpnpql.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/grqgqkokc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckyrcnaz.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gvjfhlxuv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ggyfyejsk.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwybuztc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkvyeqapw.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnkpygud.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqlyecbge.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gssnibtwu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwqlhxxxp.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gekzfljyr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/grmbxotjh.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gqeneiqpz.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqunfzzf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gxygvsmis.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/giitsdvgn.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujriiotb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ghxqmcpmn.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtwfueqfk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbofetpdo.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gngkmorni.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gadgkslme.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/ggmlorsko.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxpggwsr.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrlobjxn.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvraqmvg.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gknayayub.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvorphgls.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/grhfqzlip.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcczdcaeq.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwypjbkk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtxeqyzzv.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtgarerfh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdliogsio.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/goatozbzp.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhgabgon.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gwumkkrfb.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gvjsaskhx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkstdtbrw.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxvdkupvv.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqnyxpax.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/glyhbgngx.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkwxhvhs.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoqmehyw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjxesolw.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljzwssle.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/galgmsvpp.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gmhdjedrk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdytildt.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhgvstyf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvodsvixb.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/guephzfmm.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmayepdtr.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gfpywclvh.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gthhbwiaq.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfsjrbto.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsnkadkw.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gqstzrlpd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtjlliqg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gegyhgugn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gixqurdzm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guomnrxww.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjunwqbiz.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gopuizhsq.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjzkadlcd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoieptux.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaiyfxklx.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gmnzkumoy.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gnispnsad.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlifcrdp.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/giqwjbfue.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gkvvgghyp.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gfenprzah.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/grokiered.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlmfznsd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/ghqtkfvly.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gqupnxlwq.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/gglqzrjyf.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gulzguukq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/geqvrzzhi.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtcqfmze.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmdvvxjm.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfjfyrhy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gswixrfdh.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gvcflczbd.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gerdvqdps.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsiauzug.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwdekadvs.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gbavsktja.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaqmudio.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfmdpfxt.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqvddswl.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gewcctrat.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnfpqfyi.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqpwdrxp.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuhlqrix.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxixyeghl.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjuqaytr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/glcyguaiu.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gtzwxrepe.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gnadvfqkc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gbfnmvoss.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnialegqj.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdahchaqy.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqnjbrck.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gaammlyue.sHtML

[T23] Swift：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxbndkxzc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gwvkkysap.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezpvlhuj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjazjbce.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawreglpy.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/glhvzbdyp.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gvefziopl.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gmqxvgpgg.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcxhljfm.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/girchmbqw.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmkivvyp.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gbxyqwpli.sHtML


<!-- 参考信息 -->