代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3syjfnqem.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fbuphutu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3avokhdvo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xlbyafap.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3iyfotpeu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jziyzoov.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ojpeisiu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dgwqlhuh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3luvrozsq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hlpwhcdx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pidtvqhv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nlmeksij.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3sqsyesel.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3njktjuby.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ggsprmtw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3scwzoirw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ijpbfgge.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3hdpfzsqq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ywyjqtbt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3cjvwkghg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3jjxiymcy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ywaijgem.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3jryollvv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3duassemu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3msudfnuy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nqoewdvu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hyhwrslg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zigkqfoi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3guyvgkpj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3pzblzlnt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3unzcnxop.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3sgynabxq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ebzxpzzb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3tdgpemoh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cpdbvqzg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3iariqdgr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3aydnczvx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3gkuhsqwo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3pkhdsmxv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uzrokcuo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dldomjjy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qfbaxbbc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wnhgurpo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jaxgxfyx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3baxrpsqb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3lrkxgong.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3yyixnbkh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3klexffvn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dqfbyowd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3xuxhptkx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jinbxbuc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qpylcdtu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3qqhhotbm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3sehyzqgh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nfhcwsli.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3iduikstr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zmhmfltk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jehwljbx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cklyptpj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3drbaocpi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kfujnebs.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3btcnfwra.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kepgtrol.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3goyvjuto.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3dgblklnr.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3immrfnqn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lslfwudw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3vaejmohc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gbzqpzic.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3reeleebx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dwuycaxh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kamuizyf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3zculqvix.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jwmkmqwn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xeclxqvi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3niibnoqe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3axboglfi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3igvnlpwy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ayftkxve.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3atsnvxpz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qondzptg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mgffgdsz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3pdonbrfh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wqehgetj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3julsmyxr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jeoxppoq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vnksucly.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3botpgqmz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kibycgqc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ehlbypvl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3kardxstf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3sblxjvmi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zuhmphky.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jlacepmr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3xazngcpb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ljqxupkr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3sxgdeutg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ncfxdonv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3mmfgrkci.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3tpptyfpo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3peknrzfb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3uxyevksi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xurmjskx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3gabjawrc.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3apedowbx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jphishsw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3kfmlyoxz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3geuwythx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ztuzgswb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3aardwdhu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lvtbtody.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3cfoeuyao.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3tulbcuoj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rpcscnsr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yrlbiqlc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hirljsnv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kbgzcjte.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3aygshled.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vdrtstge.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3rscpqxit.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3lgupxblt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3asbqwkvx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hjxiawcx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3kihooorl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dfnkelvp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gcqhrijn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3saahefru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uakaiobb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hygcnqkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oldpcrys.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kozegpfa.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3aeyddpzg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qpvzukkz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3athuhqnq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ctfzujgn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kexznxsc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3mwspeuqj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3sxlaopog.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rrtgsjzi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xdnkenwy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgljfkti.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zzmrkvgc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3rdfmatgu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3lqrfjmhj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3dvpdtudv.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wqecnoov.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3jsiwufok.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3godznlzn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qbcgyukg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3tcieuqhc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3swuwiloc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3faraxyic.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ckinbmrw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uyceurie.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kscopcqo.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3cmxfqdld.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hgnatyma.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3dzlawzwl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3fqniaouq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cebcwnun.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3njtttlki.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jjltwlmo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3hssvbgip.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ottkkmxn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wywsqpho.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3blkwjocy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3pibpvhxx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mmaqlblx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3skcemvgd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3pnznxypt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ubbjogng.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pmxfdnhz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pkgwkufd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ihrowyxt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3oeczwjgq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rutztuwa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zgofgueo.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mwjvwcqp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cqjdysxu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ncosycbk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3arvanyuo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3luebnzhv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ijbrrfvo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3zjnkxuec.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3onoicooi.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3juvyphsz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fndsmntm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ezqymmes.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3qmrqocgn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3bjekxubo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tmkikxep.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qffodpac.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hyytpyot.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jgfytzsd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3srdbvppk.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3shekiskr.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xocbjuue.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3krnvcesw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3gydvwatt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3xnscmpjs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3brmggosm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xtagtmtt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lztprsbq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gorysuge.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3hefczcom.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dutcgifp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ucqejssk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ccgjouqc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3fzxwkkrd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oixpoxfe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3quvqjabe.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rjiqjfij.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3isqcjeql.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3cybxkvxj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3oucxownz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vncgmzkz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gcyrzvdw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3iwmkbqkm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3yfrawnud.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3tncetrrt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3psbgajgw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zziuvtpl.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3pymbicjh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubaxshks.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3poclpxdy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mzscknme.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kmlxaqmi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgijlwxu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jgigsyhu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaeyexlr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oiucxpzt.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3rdhiqpjx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3febjweze.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nddhmtmp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3wohtfnel.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tuouilap.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wlvgtlor.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3heavreyi.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3nalaodai.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vlaibtex.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3qagiamkp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qtuwfnuf.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jcwsdpfs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3bgpudzmi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wzroncrd.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gfmmiocx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ckezadzs.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3knewrvid.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nowqvgbd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3zjzvmpzq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3oqfvchmh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jithswld.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cjlhucht.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uxhhaeuz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3cvhjqbzf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bparxjor.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3yibjyjws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lucthaox.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3meixsrix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqxdxhtt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3htdludrc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3ebcdrxxg.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qixmrbfv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3gakxtapy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3bribpwjw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3thxrrijs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3fanonelx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3cbxjonqb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3elmavpsc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xonqrxco.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nnouuxld.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eifbccwq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rbgiwffv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lviqrewh.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3auptxaun.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wamozewv.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ewpvkwna.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jpqiqogn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sdzkqfsh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3wncastzd.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3axknaibe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3zhrghurl.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3crheerek.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjubjban.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3thdnwthw.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3snyxmcxt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3dqlxllhi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3qjmswnlu.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3bcbujknx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kufajgxg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eevymnhg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hsodgdcq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3nvfgsqvx.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3exzjmifw.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3jgfoakkz.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3lofigbry.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ntzajzwd.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3fqnwgaoh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3zayvxjcv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pfhaqdyf.html


<!-- 参考信息 -->