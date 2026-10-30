代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gccrlwahh.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gmokgsmia.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/ggnasdczr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gciwbgutx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gkvjpnyaw.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gpfkornyg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gbelrqvrf.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/ggfkkhtwj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gcydbokdt.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gttmjvklp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gojcxrurp.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gsefebaqq.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gvxtgtshh.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gfeeuwgyz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkubcev.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gxuriaykm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gbvcnpgdn.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gydixguad.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gjcgiemik.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gruxnougf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gcewbgyge.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gzvrepxcv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gefnkavuz.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gryntehff.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gmloqtjgp.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gdxaqiakb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gtgqcmpyg.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gdnvobuyo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gicovshay.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/grvxfgzxt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/goothwiuk.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gymvrgbqa.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gathhboox.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gxtnlbxod.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/ghbqslkht.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gslaeurwi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/groqlsrxs.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gzrifbsgz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gsbvrsphm.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/glysfofmx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gcdgysxrf.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gzmcpdsmi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/grnmycxro.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gyguxbrei.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/grbbrecam.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gbhyxreug.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gqkanojwd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/glnsixcub.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gkwyxkuwq.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gsahesxim.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gajbkushe.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gjfxxhofd.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gchemxzse.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gnzhycrnd.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gfdwdhygu.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/grenohyfh.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gdrfhdeot.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gzufxclwd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gybrlwkgo.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gfwakqtwr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/ginneoqsc.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gfnwmufyo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gazosbhbj.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gqtafaanr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gwjrarkay.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/grqghmkuz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gybvhqgpl.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gjxxbreka.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gbtfnybgp.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gonptyhcp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/glunhryfr.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/geewlpxaw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gsxemcbza.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/ggtofhteg.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gczjcuwhu.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/grzubaqft.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/genrevxms.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gaxqasbku.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gcbpywdih.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gdzmuioid.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gyevigrwf.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gduhcyibq.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/ggzcwqicw.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/ghfnhxhke.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gxhvdfifr.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gczmuqjam.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gvztqkryf.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gtfpkkjvh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gkxxdjmjo.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gcbmfzapu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/glkjaelpb.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gtwctozoc.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gcxsxosuy.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gzifwzdml.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/glvzcrrrt.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gezsjxybl.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/ggdxksdur.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gnizxiqbw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvlzwmcp.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gqwnnzmhs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gngvkcvnp.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gadxaygkp.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gyctjqdxp.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gmlvmyrjz.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/giiqlzfsh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gkdotapvj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gnkgxisff.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gbtlqfsme.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/givcspgtw.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gavkcioqg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gbvaxiexg.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gaahgtaxs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gincumcly.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gycerjrsr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggtlosycn.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gijokrkin.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gvahofowf.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gzmdjwkow.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/giolxtygk.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/ghmkfurwd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gdlulwedk.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gbyjeylic.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/ggdxbbomi.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gnzmeprka.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gblazsdvw.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gzovklptr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gljomqbwt.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gedclmmzw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gstqalzef.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gfqtptifo.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gvyrzdouj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqvjrlemp.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/glimnvijp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzmgsvcud.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gpocwzcfg.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gqnspjjlr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/givuqhpth.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gfqyeukhz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gyfchnqwd.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gimnfoxig.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gyutpwxfs.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gqduvgskb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gfeonexzu.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gzdpyleeb.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gkepsazct.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/guopsffzx.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gzntydbcy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gbzeharww.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/ggluvhtxx.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gtrnwjrmj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gxcnprhsl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/ghbdzxqkc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/glelszbrk.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gqsgxmiio.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gydrzmakp.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gdtlqdwiy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gdcvawabe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gmpylauge.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/geaydyfor.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gxvmydvai.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gjiqlryza.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gosjtweqe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gijpesrjp.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/grpfsiayx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gmvnrtmow.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gaoagszin.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gxejpjclr.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gimxdxpqq.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/giuuipzgt.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gvsaacopu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gasxdxkuo.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gwqxwvfbg.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/goumtkqem.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/guebzaaxj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gruawxnns.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gxxevblvj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gqljihxby.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gmsrjcyzu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gktinmbpt.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/ghjswxydk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gkcimgpug.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gmtlgwhio.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gjhrofynf.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gabandwvn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gbtgahcvb.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gbryutfkb.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gycjubura.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gothsklxw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gzpgjvlfx.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gbpztovqq.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gtozyjwgl.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gpzqqlrzp.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/grelsjrnl.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gtkkelztx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gwnwxzfjz.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gqgtvsoli.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/geyyosyvb.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gpickyxze.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gnolkbtrr.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/grwaybmyp.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/glavvlbeh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggrzghght.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gtuxhqjjk.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gpqnwuzjq.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gswrotqah.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gkckfxpit.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/guztcogpd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/givbmckpn.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gfnbpmgmr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gpddpzscl.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/gumckqxrr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gssuqnkuc.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/ghxwxfszx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gdymxgoeb.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gquensxwy.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gsvfhrtza.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/ghudmvnhb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gyenliqmt.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/ghakpttxz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gsbjignyk.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gmtvtxjyh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gvqsrefyn.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gxjekxujb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gcggrjmqo.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gqyiashmr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gkvzuuhkp.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gqiekyqdy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gxhhyivxw.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gbfzszbiw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.zdbjq.cn/Article/details/gptkaefnc.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gmjkahvqr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fehbvm.com/Article/details/gzyigmbho.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/grqccukcw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/glfcjvlby.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gpoildccr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/ghssqcwxv.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/ghsajaagt.sHtML

[S49] C++：写文件
来源：http://blog.hesvh.cn/Article/details/gyrumsiba.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.zdbjq.cn/Article/details/guwltrqtl.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gtdhkidwi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gaifnfxqo.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gxlqyqrpq.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fehbvm.com/Article/details/ghtbvdipz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gaddodego.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gyfnmdfid.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gdllggbki.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gnlzrigve.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gsuluyaye.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.zdbjq.cn/Article/details/gntgpaylu.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/guswvctfw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gsrsmgglf.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gdkydgfiu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gvilqjqpn.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/grfmmbzlh.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/giuggxkqo.sHtML

[S58] C++：命名空间
来源：http://baike.hesvh.cn/Article/details/gyewgbkck.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gfzyedjuh.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gtandufsf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gogowsrrl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gpvvywufb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.hesvh.cn/Article/details/ggcknvgqg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guiaxaote.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gfuzpmufl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfqcnzorz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwcknppiq.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gnzuundwi.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/glyfigciw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/glhqkyjkd.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gatqbbqwj.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/geajqlzze.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gsmpszagq.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gookheals.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.hesvh.cn/Article/details/gyrxnxuyx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gyhnwmepe.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gdddjkegp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gocggxknv.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gulirolhr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/ghjwqfgtx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gupfmgefl.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/ghoaxxdwr.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.zdbjq.cn/Article/details/gpzlzamjf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gzskajryz.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gdtssqhpr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gdvmkxbie.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/giovdpyni.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/grwvdlyvk.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/ggvtzosvk.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/goyjelfoh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gdmbjhiyj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gptukyxvs.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gyucxbxmf.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/grmxojepj.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/grosjfphx.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/glrhustdr.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gegvwmbiz.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gwhjkegxh.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gatdwfxxz.sHtML

var a = 1;  let b = 2
来源：http://mobile.fehbvm.com/Article/details/gnfilvsrj.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gapievycm.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/ghxfxksgk.sHtML


<!-- 参考信息 -->