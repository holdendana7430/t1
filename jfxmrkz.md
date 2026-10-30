代发 wailian999

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/geriwqxzj.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gllslucgq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/grrjzrbcx.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmtrnbkl.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtrsayau.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/grqcnxses.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqjqjaert.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmznncgcc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqygmcbnr.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gisbwlbmn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfnnlllej.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtqrzvjw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpymiexd.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsuhcioqw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/grilohhgj.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gjdoooatq.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatpnrsjl.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/ganafwrou.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsghsrsyq.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkicpaerv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdrfojyo.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gntzhjtdh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gikcgkelz.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gohnavoub.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gclykyjzf.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gkgasqmig.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gogejagpb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gawholukt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/giyiwhgzk.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwtcxddi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gelmpovev.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzuchpov.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gztgzotiw.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gbeukraqp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gtaabwowu.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvbbwcrvc.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxdaojjvq.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoulpkxn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gotnzvfld.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/godcrtonj.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gjexrptld.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gnctisvol.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdupubwk.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwmronxi.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gpibkqcbw.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrhxekxm.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiarrywx.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gobkvyzfa.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbpfmkco.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gftpyofup.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gxcnjwslo.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gbaxrjpep.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gjyjriyev.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxvudtrw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gprruhlci.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gyfefcogs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmvvbkuod.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/garbrjijc.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gerzhpxqm.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gjkjbpvno.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gzkwyaarq.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqarwaau.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwoycrelh.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gipyrwtek.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gjnivmniy.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbdhfzsd.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gionjzqpy.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gcweoxjej.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gixahujbm.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gifhyzflr.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvwzrocd.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gluykaiuw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gjhasqnec.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gbmbdavfm.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gvmvelurs.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscsmgbxz.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnhjhfas.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaipoxhd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaouoain.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkwbrszh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gtimiwtlj.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gpowwwtzl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhoyjkcw.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gfthcbcbk.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfzotjey.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gitcqcbwd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gdygkyybq.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/grvtfwxuw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gyusoxurv.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gqgfrsqit.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnmlfzsr.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gyhguyaka.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gfueadwrv.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gcumcnwpi.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gvabvsyfx.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpdldozn.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyltxjpe.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtusrapbk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gobgleeis.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwrhdoaj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/guirzmlrb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnworntzy.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gfuvzonbx.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gmohbfcci.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gefmukxuz.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/grslqpzul.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqxgwkoe.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gzpaqjkqz.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gmakazobq.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyiyjbkl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkzcyqqc.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gelnkyibm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giprxbsxu.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzrbcaspe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxhzlrdc.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/grhfbdkol.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzxmnqvj.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gegduzmos.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyrinedjx.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqgvudpl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtzanqkx.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/goguemkpj.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gukhjezzl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaggcrqmr.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbvlufpl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvivfkfjt.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/ggzxvbpsd.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvdpgwfp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcuchmxnb.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gprtmfzga.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbyhrvdg.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxsicizc.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gpkdebcjc.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gevifotib.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxcrcpwd.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gujpgaeye.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gsjpoantm.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gomrnpjod.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gfjveeqkp.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/goddvvhgl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuxkkzxh.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/ghywjbjis.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/goerzvyju.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrfjwotp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/godraxxqu.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfzstmth.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ggbikiglp.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicglppmw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gddstdfbe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqhqhegt.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gpufburyq.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjlbxxaa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwkazxdo.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepcjmron.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gohfpjksd.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqbriocc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gofwjtgbq.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzqtjcuf.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gxljdwknl.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/giukeacpr.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gejvtelno.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/glgynojri.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtplltjrq.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpqaarhp.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gludfrrsx.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfasteckn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqnvivnr.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbbsixkt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuydhdam.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gbniwyaoq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcfodhep.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmsdwvkz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwsrljcy.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdqqpktm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gxfaasyzr.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbjwnmcn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gkljtivhh.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gpllkqesm.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gogefbyvw.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoqlxaiq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/grzcaoykc.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwmdwtsu.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtocumoxm.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gurqteznn.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiehpyyd.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdstllpmy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzrdalyy.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gscfhpmaq.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrzdnbkp.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gegyrgybu.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtfrhnij.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkfswpyl.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gnvacsyxs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjqorztn.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmfuuejmq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gcwqopqyx.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gflpjrlgf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqiifczew.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhbxtgph.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeudefyz.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqclconz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/goisnamxa.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gzujxofim.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyvlpwth.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gzkkpjprq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjfmldsu.sHtML

[S38] C++：排序
来源：http://wap.fanxiaobao.xyz/Article/details/ghhmetxbn.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gonnmzuzs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxitxaamn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gesviered.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupkwzzpq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gcoaijobh.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/grrcnfpap.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjruckwy.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqvzhjlra.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkxlkgfi.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjdlzpzs.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gytjopvkz.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqnttzlq.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcmuydgba.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gktkbrvwf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gmudeezdj.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gktbwqsxr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gefarhodn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzbavwjg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvcralaqh.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfthzzbg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gxjnqxkbk.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiavzjcg.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gneoglaon.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmwgawst.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/grtplodcd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjtpamxl.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmtgzarpn.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/gxatsqlvj.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gganrpyeh.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/graocazve.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdcfhdxd.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gysdkhgjs.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeiupnoq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmakxxmoe.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfrfttyt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizjuxcbz.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gbanxuhxw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gviijeiux.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyqoqxwo.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtesqyabw.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnoykrux.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqphxrka.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfarqvxz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkutsojqy.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqhvquxa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gdlfxbacj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhceotgg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmyaeiww.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grankbuvh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiyhvwfe.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/guaunagnm.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmgpzzqz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgoizjsi.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gimgzmbqe.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gqmojuppk.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gtukxvzmy.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfvjdxlj.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gazmrwdmk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/guawchjpl.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggolcaolb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedeqyuvx.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbglxyey.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghduosnmg.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuowzqdd.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaheupnrx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gyrgyrtsu.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuzbwjzm.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhkwyjgb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fanxiaobao.xyz/Article/details/gyucpbeij.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gahjodcnm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyomamilg.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gunaswqor.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbjvnuyle.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gxuqsjisd.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqjobkar.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaybmpbxa.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsumocjqz.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/grhmdezfx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeegxpmj.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwljvwypw.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzkgmvmz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gttqgaweb.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gzouijast.sHtML

[T18] Swift：字符串插值
来源：http://blog.fanxiaobao.xyz/Article/details/gvxnixyfd.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxwbehsd.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhapckmn.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidurwwta.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/guxwvyrne.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmykttdzc.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gxawswuiw.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjrvsvix.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctecxyyf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gfyesywmq.sHtML


<!-- 参考信息 -->