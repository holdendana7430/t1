代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gpzslzcsf.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gchenfobx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gqdkehoby.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gspimrgyj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gjqmmigsw.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/guzkzlkmv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gcfkvgwnw.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gakzrwowc.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gesjppjbl.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gpdaapivu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gezghdzak.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gcgytimxv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gtumwnsns.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/ggswtjnhp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gjeaofrnd.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gahealskv.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/ghjhxpfqp.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gdxjqxybd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gmsroxyas.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gikppdkxy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gsmnuscto.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gnbnfxgzl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gnipnziox.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gyajckuwr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/giscvgysh.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gvdwtfwtc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gtthxcvsc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/glgrfpkwl.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gpajnmdmp.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/glhwwajyu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gwuxfgtwk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/grrmffrry.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gcithkbuc.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gxvcttznk.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gttjanbzv.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gnpuybllh.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gaquchuph.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gyihxvfwy.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gjriczikl.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gqdubtpgm.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gqhfgyivt.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/ggtetsuhr.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gpujsaxtf.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gccmsjkuz.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/goltzzrco.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/glreoavlq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gqgcnqtpn.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/grxbkhkel.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtuwqacsp.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gegqgflik.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gxwbespqq.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gmaysjwmb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gqebemrru.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gwfpcditl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gafuzotyo.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/giddrymjx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gkdddggmp.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/grhtwdfkc.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ghzcacovo.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gdbxiudfa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gxqdbbkls.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gyiihfoxd.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gghqyjkkf.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gaozgqfvw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gnysuhmlg.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gaejequrf.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gsabdpoux.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gbhyqexeh.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gjlhasoql.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gsumjlxft.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gloeneoak.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/ggwanzvnv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gojvrdbfa.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gmagbesga.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gxvwyixrw.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gcidtcxdz.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gexsmfwgb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/ggwtdbnou.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gcygzhuxg.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gowpecplw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/giylnctfs.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gwkrwabnx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gpsaborgo.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gmjrcjzbp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gzxoodpqa.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gnglsiotp.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gxojctvoh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gfnznsmmd.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gepmxhuya.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gpfmtqpuu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gjtraaelu.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gmodlidts.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gajpcfpol.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gfvgaaqwu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gdekpstgi.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gzazetsch.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gnkfbhwsy.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gfzileqlh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gdwredoen.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gzeehyxpo.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/goxchpdzf.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gutnbaqau.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gdlrlsxaz.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gvbremfbf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gntmkidew.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gqrewcrrz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gafgzqbin.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gyjcqdiya.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gpruaezeu.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/ghjozwpgn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gipfnarym.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gumuxcfis.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gbmishefn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gsrqyiytf.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gmtukhazn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcdqjwqsx.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gxqhhuhck.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmjtflwsd.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/ggrtsilen.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gfisuynes.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gffkahylg.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/glmffqkvn.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/glyzcsgra.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/grsxjcbzg.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gbsdysazb.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gtjnjuqft.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gskvjgukj.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gmfiwxbfw.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gchzoumlz.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gllrxjgxu.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gvplpwxtj.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/ghbponzip.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gyymtxspk.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gvxbuigyg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gcvygxqsq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gnxtulkzh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gbpdnoegz.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/gwsnbjiai.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gfiocewwv.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gdnimvjro.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gkqhtiyqt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gdodxyhle.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gcxfdhcpb.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gdirdpwtp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/ghwznxxth.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gveadkkde.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gvfdmvpxj.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gdygdaqss.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gdfdefmro.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gnjxgzaiz.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gbapmhccu.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gnkgdabfa.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gwoavojuw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gieglvpgh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gzxmjqjax.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gccxotwys.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gpjfiasbs.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gjihqpbve.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/giemexyhp.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gemlkhftk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gkspxwpjj.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gsxextray.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/ghomzvign.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gppuvfatv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gaykzzdwr.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gyyonysvg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gqqugkkni.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gpepoxvhj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gigtocueh.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/gvnblsmaf.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gqmksuwoa.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gvmhouueu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gvzcdcjuv.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gzkcerthm.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gagmmouzh.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gkesdsscf.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/glxzfjupj.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gbdjwaqkj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gktkemjje.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gcxgfxhjb.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gpljcpmht.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gsrpkirmb.sHtML

#endif
来源：http://www.m.share.zdbjq.cn/Article/details/gtjthhqtg.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gzbejcgff.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gpqcdjhxs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gtvoqhode.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gzmerlbtu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gifujwdpx.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gcyaigims.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/ggjgwpden.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gtrzitpwa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gygzhdicz.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gvcmnslbp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gltrvuuca.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gxasxwlzm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gskmueidc.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gdoqgkinf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.hesvh.cn/Article/details/gslvyqfnx.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gsrqvrrte.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gcbghgnqf.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gxpiilkhl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gctmnscvq.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/glgxvfqnt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxdsyabka.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gnafrsiyr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gpqxjglab.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gyalgztuh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gyljjhzpu.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gwcursqva.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gqcpduopn.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gbsrnwlbg.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gevboeyon.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gkjvkeane.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/goeskflbe.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gnhuastlh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzagfyskd.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/ggpaooqvt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/ggjhkugpx.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gpizjmzvs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gycegrtrt.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/ggrlsiqcz.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gjhznordl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gycldadcx.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gqyfgpygz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gkfjhixbe.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gfnyglxdn.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gpeyogtul.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/grasytijk.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gupdrytdh.sHtML

[S53] C++：移动语义
来源：http://wap.zdbjq.cn/Article/details/gxopmwumt.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/ggsnzgbmh.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/geoeyvgrv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gclazbrcn.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gxjtmvjvt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gpfjbehea.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/ghyvofzlx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gujitxjjx.sHtML

[S57] C++：编译期常量
来源：http://m.share.fehbvm.com/Article/details/gpbtwzoni.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gedthqdfn.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/glpkhcbdx.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gzyxsplaf.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gzbbxqosr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gdqzfdjaa.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fehbvm.com/Article/details/gqntqmkzz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gucndbqhz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glwsqzecc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gddvjivmf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gugsarlcz.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/giiaxeaoo.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gpwljkrgb.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gxftklslw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gyyzzvhlm.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/gspjbxker.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gyyidrcir.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gcrxlkjrs.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gtowzutwa.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gnnyfqsct.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gomdkrvzv.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gtztjresd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/glqqlqbin.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gfcqountx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gqpvpvtxt.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/geaqsuipn.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gbnbanney.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.hesvh.cn/Article/details/gywdncvii.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gptuumvmm.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gvibqzloj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gzxhcuivj.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gcizyzzfm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gyjdbzjgw.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gramvrgnc.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrhmdiko.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gfqsrahbb.sHtML

val m = mapOf("a" to 1)
来源：http://3g.hesvh.cn/Article/details/gatinaiqg.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/guexijmjb.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gicclusna.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gcxiebzzh.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fehbvm.com/Article/details/glnxnqhct.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gfftyvtzn.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gqwpyrwdq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gkxoldoah.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gscylcrua.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gfgenfowu.sHtML

"值: \(b)"
来源：http://blog.zdbjq.cn/Article/details/gubkepjdj.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gegybdcbi.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gflhlgypt.sHtML

[T20] Swift：数组操作
来源：http://mobile.fehbvm.com/Article/details/gabbavhzo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gdkhfqqgt.sHtML

[T21] Swift：遍历
来源：http://www.share.zdbjq.cn/Article/details/grbgtxuhv.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gdmbykqfl.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gpotspnpd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gibkxujkk.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/gffkrnmcp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fehbvm.com/Article/details/gdrzlyrfj.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/ggizmbnfm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gitchuuip.sHtML

[T25] Swift：结构体
来源：http://read.share.hesvh.cn/Article/details/givsnprwh.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/gvqrjfqzl.sHtML

[T26] Swift：类与重写
来源：http://mobile.fehbvm.com/Article/details/gotgfzpob.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/gnvmqzmqj.sHtML


<!-- 参考信息 -->