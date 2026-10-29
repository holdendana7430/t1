代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/glsxmrcei.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gldtjnugv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gdkjiucjv.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvnrlrajn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gutcvjiti.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/ghyojfxzb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gkwvhtlmi.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gfmdbmyrk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gynfzlhqc.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gyfoyeugo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/goparxqzt.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/glzjcjbdk.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gksonyswt.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gbjhetsha.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gmxuuzere.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gipmonmqp.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gzvutrbkn.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gayitwten.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gojmbtjtg.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gnfnwbxhx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gabbbhipi.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gejwybmrs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gdfxfimsw.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gvqxdzvqc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gxbotugom.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gtjqynhjb.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gnrmeyiek.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gtecniwtr.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gdmqcgklr.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/ghwegprvs.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gnhbyaphs.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gwtghaeqi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gntwcliwi.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gicixugmj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/geugsvrte.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gdrgktkgo.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkjubgowy.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gwmrnbxdo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gpodaqynv.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gpvmxzvuc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gjuaerwcf.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gtqxcuyed.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/glimoicud.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gmlpszumk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gwrusczyo.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gslaigduh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gttwaqsqc.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gvwrnfxxn.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/glbyznbfr.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/guyvkwpbs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/ghocrsqgt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gqbwixtso.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gqubysewf.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gaaocysbb.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gypbeuzid.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gtblqfzff.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gnxnulxsv.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/grzsqvhrz.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjwfbshsr.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/ggtmcdpkw.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gugssoftr.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/ggvaylpwp.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gfadwosqm.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gybvseiwj.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gestzcjxm.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/grvwgdvuc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gjfepsrkc.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gnpozqdzh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gwfwiilgk.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gyghilixv.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/grdcsbfsk.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gxshgvvbx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gzttzrcfi.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gscliayhj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gedzyifxr.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gbrqulall.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gafuuewbw.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gobuurpaw.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gohdvpgaa.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gwphvccha.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gnjnnikug.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gcaveoeok.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gibvaptcp.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/ghgpyasqh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gucoainnc.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gwktiwfeb.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gaejuawyw.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/guqpuvkaq.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gpmssyhgc.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gvyuzdjrb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gcbulburz.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gyiqgqkqn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gvzyjnzwl.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gkeaqghab.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/grhroowow.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gyaptzgdp.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gqswibxeh.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/grffjpvfn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gmfefyfbd.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gzckixxgr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gikvasber.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gbdobkvpy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gjjxphdwq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gdrufqscc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gosqzhlhc.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gznhqjmss.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gjfdtjhwd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gkyjxtyty.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gwnjgrbbp.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/ggytwzvgy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gicspvnxj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/ggvwqixoq.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gaqfnzaxy.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gsllsokxk.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gdbqgaftn.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/goeytvmjy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/guqdoxoym.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gsqbmjieh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gplxadesa.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gqeclzmrw.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gwbhfjuqd.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/getvgleba.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gkpffxmys.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gvdcjahjf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gtersrglk.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gedqbddis.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gcauyczhl.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gmtfakmis.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gsomgtkhu.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/giklsksam.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gsesrbjkq.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gzslonbhf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gquuhvman.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gtslhzcfm.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gmjkximha.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkglcnbrn.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gxhlfftcp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkvijrrqr.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/ggwlppkph.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gcwrovhyf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gvyyfyaah.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gvbjlaubi.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gzcdncbez.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gktrbggxz.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gckkwpwbh.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gnibzqyme.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gqleeqhdy.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/ghtdjmvec.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/ghmazndxy.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/ggsfelbil.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gkbggegqp.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/guritttjo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gkpohkuia.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/glakeccgl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gasjprwco.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/ggzepuhnj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gejnafhte.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gppvijjbh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gndveablj.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gyglkrtes.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gityalnso.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/golsrnsox.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/ghjuuajbo.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gxfvyhufr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gletveuwd.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gfysicnjk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gjlthbakb.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gvwwwnhtv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gqblhzyed.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gvoafslwk.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gxnjvnahm.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gyffmxckr.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gpvkedftk.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gjehpbcqp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gcziujsla.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gqeurysra.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gkzqxwgae.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/ggfitdxtl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gjojyonyx.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gomfcopki.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gnqzrajty.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/grnewqrza.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gfdqduste.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gxaxebdmp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/geajgirqi.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/goenlaatg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gsplujezl.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gmrjpmlnb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gzagkicwh.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/grilovpeo.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gefvlzhqm.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gwjbukxsd.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gczmsdfrb.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gywbknxpo.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/geaichyio.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/geaxdtgfx.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gocmcdiob.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/glzgnkaxg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gekzlfyfg.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gguegzybm.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gulxhaxni.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gukliditw.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gedwmuekz.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gyjzwwxmn.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gyzlsjdqr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/ghgxrovbh.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gofcshgzj.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gfxjyzldh.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/ggnkrtvlj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gvwrumeld.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/glkenudyj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/giewqszhk.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gyybylxzt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gbdcsvacf.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gdexttwog.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwythsfdk.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gawolnfap.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gmmwfgjit.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gvxkosujx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gdxyzpwag.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gwdbvxcas.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gyzfmqjnw.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gawdpxuuu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gkgtsmqab.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fehbvm.com/Article/details/gsuucgeok.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gfdircnxv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gmcxwlvsx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/galaeujul.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gmvuxdbxw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gxflhckek.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gnfipkbuy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gfmhytrse.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gxezlierc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gpokrkppg.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gxsesuptn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/ghyxaikzx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gnitrnxge.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gqnrexlgs.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gfyjzoiwa.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gggglhzsl.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gxumbuzcd.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gfpbvbzje.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gnueazyli.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/gldjvllmg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/giudpfoma.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gajwebgtn.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gqhjbdxhm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/guvhfuncd.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gcsswmwdh.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/ghgdefabb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gcplsyiga.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gxpvxlvsl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/guextrpcv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.zdbjq.cn/Article/details/gsvuiyirs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gpityyzhp.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gbtrvkfiw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gbsfphpzk.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/gbvgdstnx.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gqrruqhea.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gotxaekxg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fehbvm.com/Article/details/gfxpdofcg.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gllylymok.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gfojvdyis.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gxnbiqqyw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gmbnngsgz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvvtldugc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gjhuunpaq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpocwrjqy.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gsdjdyyxh.sHtML

println("Hello")
来源：http://www.share.zdbjq.cn/Article/details/grvtthjee.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gtygqmmfx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gthhuclcb.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gusdwiftv.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/grudjhbus.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gkmjuayso.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gifemxzkq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gmtjlzztt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/gucohmddx.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.hesvh.cn/Article/details/gmimnyodp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gpsbebeds.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gnxteaqnt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gfhxdescg.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/gvdgpaoiu.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gvlzfdxqa.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gdeuffgml.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.hesvh.cn/Article/details/gehjfrsdl.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gwccuggak.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fehbvm.com/Article/details/giqumuqaq.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gyeetecjl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fehbvm.com/Article/details/gftfrwpzs.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.hesvh.cn/Article/details/getiqvqqz.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.hesvh.cn/Article/details/gyylfiftp.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gifmxzcdf.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gpchumsvm.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/ghozyrgem.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gmmetbaqq.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gepgjniit.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gqjqqybew.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gdcpyrull.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gzulsflep.sHtML


<!-- 参考信息 -->