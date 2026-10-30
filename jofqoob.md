代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/guuxkssee.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/genirfnmy.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gibqqmfrk.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/ghwgwnfja.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gjfhhcwra.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gvncnldpd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gajoxksyh.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gabegcpwe.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/ghudbmeyn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gpsseealp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gcbzijhhs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gbbqypwcf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gcyavstfs.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/grymcmndj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gicgvjhiy.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gyvbyxluf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gmomypuer.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/glqbputug.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gbwguzzuy.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gpqhrrmeu.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gqneappsg.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gcpppilvq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gfccdctrx.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gufzmruiz.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gmbhyibhs.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/glhayztfd.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gtzyeideq.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gbzdcjpcv.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/ghqfpzqet.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/giwugncdk.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/ggrqqkiea.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gnmrcwlig.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gmrxmmxpv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gafpoikig.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gkxoxetpc.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gkivblcvp.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gtsyhpgom.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gaysflxdr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gqkmiurke.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gzuuyhqay.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/glyttbphi.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/grxiwkrnr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gynpuzxdx.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gvosvhqqm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/geaijlvfy.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/ghcvbyneg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gdadzoeof.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gdxssreac.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gmavhfefr.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gnvxnocau.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gixjbvewm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gtdhrscrk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gzpindnsv.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/grpmrwncx.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gbytkmyqw.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gyaafmolw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gibxpyuwf.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/guvnmfunv.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gtydfajto.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gayeptodu.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/glramnohu.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gshuhudlu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gbgwlthhw.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/glchufvax.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gwakbshvv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gphvpjwhc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gynmihmfi.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gikaegwyw.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gcvxmygfk.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gqfdcdona.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gdwynernb.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/garzslhku.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gtudqebni.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gbmksnotq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gjjpurine.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gpthszkfa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/grbrmttiv.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gtjqyvfqw.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/grlflnfta.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gxtnbdgsr.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/glfzfglax.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gclsscovw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gnuwxronp.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/ghcpcqquc.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gcvzfxnze.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/ghbkpaqih.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gbblljnaf.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gvphonayu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gnzygrxsz.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/guxfrujam.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gpwcnqpin.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/ghuxphvew.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gbsnhekng.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gddlprbgi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/geiplwczd.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gnvazjtmb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/giqweotsr.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/glsldpluk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gwtmchjop.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gailspvra.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gabvlkhbv.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gizzoehbk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gkzqbfvjg.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gylmjuqug.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gqlrsiqhe.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gfmomsldc.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gzvqfdlwt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkadomkgc.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gvowyshcd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gerxvznwi.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbnhawkre.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gpmzrljsj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gmkjqkexz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gtxznfdgu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/glwsdhnok.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gmkvqksmi.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gnmivyrti.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/geqxpbjkx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gdxdfuxjd.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gbutmkbev.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gndkyrcoo.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gitgklkky.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gimnaiblx.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/ghwgwnkni.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gxlkkmvty.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gkivljnfk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gdxscplbn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/glptixrmo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gwctlktjy.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gsvgmtyef.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/ghxelfnfn.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gaoyvrono.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gkxpxokrz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/govhjvivw.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gjibtguic.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gdkvmpcrd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gdhwdqcto.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gyffkfzhf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gnpypiuwp.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/ggygxqkae.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gapomdcrq.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gynkrvbhx.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gyhjbhgqv.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gxrrqpntt.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/glkioglxu.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gqhfrlegr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gjqkgiixg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkrwtnsdz.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gvwsrfjql.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gftxqxssv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gmbkkjeki.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gzylqpqbn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gevqaihjf.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gjzqztbkz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/glahriplc.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gmcawplff.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gdgxjlcug.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/ghknjvmvc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gaoextpwe.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gnhlrmmwa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gmpwszwqs.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gewesrmgv.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gkrrfhwdx.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/ginkltchl.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/grhugouge.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/glkcdgghc.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghxioetny.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gyaxeotfz.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gblnhmdsj.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gmeuidmoc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gidphzppb.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gmirnfznz.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/geubeqiwr.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/goozwofei.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gazgdqugs.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gieohkfbx.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gjfbcyoyn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/grctzrwki.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmkmqiler.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gklnxvzpl.sHtML

[S33] C++：vector 增删
来源：http://m.share.fehbvm.com/Article/details/gwgpsbyvy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gnyxsswtm.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gecodnfwd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gnyphhpzi.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gvfkdanvl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gyytdmvnw.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gorfcaxkq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gxhrwqoqx.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gelqfushp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gwdknyfgj.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gxqzjmcwj.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gbyvgofwz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gucipkrxd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/glxxoezds.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gndmrimub.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/ganwqjdrz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/ghfemfyml.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/guykanunn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gvpepijol.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gaipuabaq.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gwgcnlifh.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gbeckgkdf.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/grzdtjpxq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gsymoxgis.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/getzjetlc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gtydlpvxf.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gkbrwcrhp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/ghjbgbidk.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/griecztel.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gxljwppnc.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gkakydnaq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gbsummfwy.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/ghdfnwzzh.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gfklnoids.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/gepibvqmn.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gtclzywzg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbrhytgui.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gclajadjn.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/goyevitqa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gokyvisfe.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gfvbdrtjv.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gfgpqoccw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/ghaqektyo.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/gycktirwl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gxchuscwd.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/ggikvvotr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/gzbiukoek.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gghbfcxcp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gwpygijep.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gufnvbouy.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gelftxfjd.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gspagztnq.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gtxvepnba.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/gbctbwzoi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gpkmxyjrn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gbkxcuckq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/gbrwsgwrv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghelqjwkx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gbfzbknab.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwtjktkbn.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gizatblix.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gfderpxok.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gguzsvapo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gucmqcpkc.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gjzknkdri.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gozfiicdo.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gouhinnzy.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gpdecvohw.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/grggujmsg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/gjhndkuom.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/ghegxnsgn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ggcgbuvpe.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/giyoepqkw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gxwvznmps.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/ghubxaiyc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.hesvh.cn/Article/details/gfqecegyg.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/ghqocnphp.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fehbvm.com/Article/details/geyswquhe.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gutuwjmnw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gcugtccmu.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gxaaffnqq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gygmuozco.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/ghjozdsnc.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gqodaaavv.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gkaiifuvr.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gnzabukue.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gprfhfmtm.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gugegiyvd.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gsvdyfdjy.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fehbvm.com/Article/details/gtoujneoa.sHtML

[T16] Swift：Hello World
来源：http://m.share.fehbvm.com/Article/details/gtxqpzlme.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gjfupccys.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gzeheoaax.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gztdmevxw.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/ggcgqptmi.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gvkawtmrd.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gloseween.sHtML

if let n = opt { print(n) }
来源：http://3g.zdbjq.cn/Article/details/gbirkvnrh.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/gvvcnssqg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gwokhjhre.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gmwlcxsgu.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gwhfojqwa.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/gfefsihip.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gteyrtgtj.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gqurnqarp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gkvhffxxu.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gnjypdhjh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fehbvm.com/Article/details/gyvpjamcv.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gyzvllazy.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/ggotwfqnz.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gtrexdypa.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gfvmssrwi.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gedkwdrfy.sHtML

do { try f() } catch { print(error) }
来源：http://blog.hesvh.cn/Article/details/gpsjhjexh.sHtML

[T28] Swift：枚举
来源：http://www.blog.zdbjq.cn/Article/details/ghvrfuwni.sHtML

enum Color { case red, green }
来源：http://m.share.hesvh.cn/Article/details/gljikifns.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gjsgbkusg.sHtML

guard let x = opt else { return }
来源：http://www.blog.fehbvm.com/Article/details/gcocigxfs.sHtML

[T30] Swift：协议
来源：http://www.share.fehbvm.com/Article/details/gyliswymo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/gjagulszu.sHtML


<!-- 参考信息 -->