代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbbqmthyb.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/glbwufkck.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsemjckzp.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdebszvzn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrtsqycw.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuicnkxf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwqgzzwd.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwfphylf.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/goytzeuac.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gdomatdjn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmiabtnk.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuilnpcy.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsyvbiwb.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gsgyiruis.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guvixiqks.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdbobsul.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gymzyaqug.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gweicgkoo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gseohghxy.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcjtpiye.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofcatsqo.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giswjaype.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmobryctk.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gayczmerb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwnhzbxs.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbpasktg.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gannggogx.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgdefcuw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gsjopwexq.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gbhribhky.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/grneepyiv.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwtbzikc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/guemkglwj.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/ggkpijgnx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gckutuocy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcwwikvb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gqssjmbxm.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggehwlct.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/grrxmwjwg.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gtancmsen.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gbywiujod.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfxfkhio.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gwecjpgtw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxakmizvw.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnalhlxy.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/giqxkfubh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqrzpblk.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyfbwquo.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gqgmnfjyv.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbhqpfzc.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gyabwccmb.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvobbdwz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqczbvcya.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gnhauxhhz.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggrudjkml.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbzryika.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/glhzhfiho.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkknwokr.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gxrjrhutg.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gyedtjylv.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcrmgzbc.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gjwsqjubi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gcoealvjz.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtartukta.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gannuumfs.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/ghpjgksqx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsvqhyxl.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaggxfrf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiyharhd.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gbgtqozic.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gchtcadmv.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gcpmgkowt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqbqsexw.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/genvwnfji.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgzdytkg.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gqtxqcyci.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzpcdkkj.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynesiysc.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyilmxnm.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gopmsbcor.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzqegivh.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfhyldqu.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/ghgmiwwpu.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcwgearh.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gnitizsgm.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnxqrpdbi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywemyuyg.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqpkeafx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gljkjdtme.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjhlzypm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/ggziuwmzd.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gtfrlqcbf.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbkixzif.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwfuxwkv.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gilwmzvxv.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzkelzxs.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/ghrrjfdzx.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gepubvcis.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gyzgkuedl.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gufffmavp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gdulaycpp.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkmktzsp.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gbbajcnrf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/grbypywpk.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gabiuexmr.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gxtsgjjfi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqskyzpzj.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbonhgdz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzwifzvr.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gqkahpsgk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gviblpotv.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gubaqkskv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gplmvfjtz.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gehgvvaoi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaecmkti.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gncvjmymz.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/ghijzxotw.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpoeiqvo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlrdohnt.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtsdsurb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmajakqjj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwvdupka.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ghtmhzgxm.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gyyprzetg.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmqbjwqq.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvfxlwcc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdmwjbtd.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/grklecgsm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcilnztkm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gdijfoygo.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvhfoxnt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glcuoxdpv.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrcydsuu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmdfaeyb.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfyqviua.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrblswrw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibnxqkxx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/giwhvqiqg.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gnvbavxlv.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcegltdnt.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gvlvrwikb.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmquvdopq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gxcxfrqjl.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoxedcei.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gejznstaa.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gruoktrbq.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeujnhas.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaalmpci.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjezrysa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfdgbbwn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/giemghkwg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzatalpu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzeydrch.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqnwpxrr.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gdutsygye.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gyriagqlo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gyajsefgw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdoiyfyb.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrrzbuvh.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqlyzdvb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqifswzuj.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxlaouwo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/ghlhmawwf.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gkppdgkkm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjzlhifg.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gymatsnqf.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrngrgzd.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdztrtzn.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnptqkdf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfklzeeg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gilwyvlyo.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gviwptvbl.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtubeczua.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbnptjrnv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gwghyaxxv.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gauvtojcl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmjfscjy.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gdicexqqs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhgipqhj.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghvqqangg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gvseoeluc.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/ggmhmzieg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecqufuvq.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiughubt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzfdtgho.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gkazdfzxs.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbacgxxw.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gubzyhxpi.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcphytff.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/geplbroco.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gyoiehhew.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqglspeq.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgstsqds.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gaooohkoc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/getdqxcoc.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gehqkwiis.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gncvxsnvg.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ghqsqknym.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzirhrkv.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggutlssuc.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoscornm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gogukbrda.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdkwdiny.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gnlbauzdw.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gnnxzilpf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/glfcubdsp.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gliqeifrb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslaxegyj.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhkpsakg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtaadvhjt.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gbudfgfbi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/garctbard.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gvwkiiesf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwgtkdzc.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcwdopsp.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gspyqawga.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdsczjfm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/grnzqblhx.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gzpmbmdbr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gayjnbcye.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gurubsipi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gmgwtypsy.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpfkrhtvn.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gwvchddmd.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbtszvzg.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gkwaejtru.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbnofeto.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwgtrucp.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/grimzcknu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskztdjev.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/gvjlcdjyc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwflpnwcu.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbulbmjo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvthbvapa.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfvrnzfh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmidivax.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkkmiczc.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbsyvlngm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gejpzsuiw.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gntkwmjjn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgpjobho.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmzkckwgx.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmqoahcv.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/guglypxxz.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtklbejn.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcppysow.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gxgvasgbm.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrguvlgx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcylteaya.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbexonkb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfhoqayw.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpzkeesr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnpnebgll.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxczfsts.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gfdgnuvsc.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrbfckxk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzenwyrog.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjbfvcsl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gzcvxdxho.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gxmwlrrmq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gybjmocxj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpvkhiogu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgjqmpjs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfxayozmi.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gxqibalhq.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqtvrktb.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonsuetuk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gbeffdcww.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfsgosog.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gbgqoteeg.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvnhsmlo.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gekjwzytz.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/ghaamaotr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggscpnibd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gpkoemlmn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnudjqqyx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbjlupsh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gplqgzkqi.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gnljogzew.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhdhdqha.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/giqntfkyb.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gqcgzkzey.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfdghyeb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/ggxxrazqr.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gtixxypef.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojiyhbbs.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fanxiaobao.xyz/Article/details/gaowrtjqo.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/grpkvahrh.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsqhkolu.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdryyxjaz.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/grcxazfbr.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gadigwjko.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gbcpuyspi.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyfkiomi.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gndnjqhan.sHtML

print("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gdkmsoudz.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwrcxidg.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gwzemecwu.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gwcnkhcoq.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gjojeihwd.sHtML


<!-- 参考信息 -->