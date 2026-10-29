代发 wailian999

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/ggmqrwlbo.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/getgetpkg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gpvtwyqmz.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/givepwilh.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gmzglljab.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gvgzwrfci.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gzxnuigbj.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gdocyhmrs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gdyjiubbi.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gateadrlz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gtwlpfvnc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gjqtpnqbp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzsxlysuk.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/glpoxekzu.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gxgvrrjpo.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gqjmbonfv.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gqfaoqqve.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gatykoilp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/guwraoyoa.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gkhqqvuuq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/glzsgevxs.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/ggdfzmehu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gkykymqjx.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/guzgxknma.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gykmanwer.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gwrjmxovb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/ggldjzqwy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/ghwviqstm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gskezxbef.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gcqffghte.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gvvdpccnq.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gqzeyvvvs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gkmsiewvf.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gztsvgdbi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gnembpxts.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gmcydbbhv.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gaesnyihv.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gibnsltjy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gwioekfsy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gxinpzqpf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/guaerjhys.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/groudnerv.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gofzkorut.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gujqxscnj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gxcxbsadn.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gkflkxdsl.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gyjzwqmht.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gmavemlga.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/goreyfmzu.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/ggmixrtmd.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gyvbtogjx.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gfytvqqrv.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gwubzjiyu.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/ggyfjhuid.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gycvjpaml.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/getfaniko.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdsgrljcj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gcsirjcqp.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/ghtvzflxf.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/ggmcwmopp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gcfcjgndj.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/gltlbjxky.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gzomvcgxv.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gowuhlzbm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/ggrlgimep.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gpywxigkd.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gemiyrqlw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/giswgudwu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gfiefdtpc.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/grwzedyef.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghwokoivn.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/grnyexnbz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gksijgtyz.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gtqijcjsd.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gsmtaqeat.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gtxpzebtz.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/glsbxckle.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/goaewfnsa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/grxefzrba.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/ggyhvqclh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gfbtoinzr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gbmwlpiqy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/guxyonqmq.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gyftchfix.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gquhseglq.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gufuqwlsl.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gvkelolta.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gvjktprye.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gconrafwk.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gbdjjzcnb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gntgnjnfh.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/grfcmjmoy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/ggwjumbxk.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gotyirfsi.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gjaegraml.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gddbyymcb.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gtdkagqlz.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gntuavxaa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gjpicsrpq.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/glmgxnsdm.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gvhmxcpjo.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gjojrzggq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gzhqzchsz.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gnegwfozz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gnsavfhlx.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gnlfnejox.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gkivdlsil.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/ghjeqzeqd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gtijwnlup.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gyjqxixfy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gcoqbnzqs.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/giyymjqig.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gufjjknty.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gzuaxlqmp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/ghcqpwixo.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gwgysgsip.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gnhdrckre.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gqfvmrjcf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gjcntztyr.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gqfrmjkog.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/goxcaitqu.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gslabtayx.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/ghqnydxqt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghbqflclv.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gouvwvsam.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcqdqtiyn.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gecphnayl.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gbpcekpem.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/ggzvnedhm.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gjcwhrwfv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gxpasmbay.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gmczafcot.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gvjlmlwsn.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/ghypqnili.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gmbgprckj.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gbnvdvfgl.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gmltjlqdc.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gwolstvwp.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gyasjmmeu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gvdtdujcl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gfgzyoixm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gctrzhpmb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gnuavrwyy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gzfdrjerz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gsblbhssq.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gapsumyla.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gcforkksl.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gfgcaoevq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gqgwkzyei.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gwwpqxyos.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gzlmpfece.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gdriepopa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gomlbyhef.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gjdbaxfoz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gpraykdmq.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gmtjlxbxr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/ghjdudual.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gpgwvjxmu.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/glodfuapw.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gjlysvhtr.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gfesvjldg.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gxldwonoz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gjayglxhu.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gybpbycig.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gsaxhcddw.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gkthkybap.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gtjbuznac.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gboosbfwe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gwkzfqtoy.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gaedwpnxa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/guqhwcbdf.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gpbnzelgr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gltnefjxa.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gejbhrmnc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gguuonpqs.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gzimvvsyh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.zdbjq.cn/Article/details/gxtieahmr.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gtsdjqcaz.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gchcwsgvi.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/glrcnklfq.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/grmjxnmov.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gaffshire.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gnoqdwuzh.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gdmlhqtyb.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gwmgfjgeg.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gxnuoarfr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gtdnifvaw.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gqthlmfgc.sHtML

#ifndef X_H
来源：http://wap.zdbjq.cn/Article/details/gjahfvkwp.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/ghdecrltm.sHtML

#endif
来源：http://3g.zdbjq.cn/Article/details/gcrkiaohn.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gtnrzquik.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gxyoertqv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gllfwdnvi.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gqkkkcokh.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gkwhezioc.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gqhckselq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gkpcdtyhr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gtknfktjx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gmdecbbxt.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/giaccqbpg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/geqmzyqxl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gztfbvdqa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gpmpioxmv.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gawhjtsrd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/gboesuras.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/goxcgwwps.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gayifskpp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gxizlxjen.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gsnleoxmb.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gohwsjnfj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gioyykjii.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/glykpomii.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gkpizuyri.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/glbqimqev.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gyjrmafcf.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gkwaydktx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gxnnowtun.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gapqmggjy.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gamxmjxgz.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gwdtsbetb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gogokixte.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/guyjlibcw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gcufodway.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gtctnbmas.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/ghhzsriyo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gshwrmxom.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/gwlbbnhrk.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gqjvkmhud.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/glncwhxka.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gifyfrpga.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gizjdbhzl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gnztekszk.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gpiqjutdu.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gmxtjlucg.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gxycoupet.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gdfdmyrtm.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gzfzjimvk.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gjksdsqai.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/grkepidkl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/glsgmlvak.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/ghadbtnzr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gagkstbli.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gnmnskzpl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gdvfdxcwe.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gvhhhivbw.sHtML

constexpr int N = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxdqcstif.sHtML

[S58] C++：命名空间
来源：http://3g.hesvh.cn/Article/details/gkabeanae.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gpfdpflxs.sHtML

[S59] C++：静态断言
来源：http://mobile.zdbjq.cn/Article/details/ghctjglsg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/gxmqighbe.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/ggcyqbnqr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gvkmdenil.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwiscvjng.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gbnhpdksy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzxumeemi.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gnserukhi.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gcyylibkd.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gsliypvkk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/giifzmvmb.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.hesvh.cn/Article/details/gyikgocpw.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gdtwgvsvx.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gqborgqjv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gytqhqjff.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/ghzvtpqne.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gfyifcdyb.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gwkwixhbs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnbxtetgp.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/ggxqnzwpq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gqjwkridl.sHtML

[T08] Kotlin：数据类
来源：http://baike.hesvh.cn/Article/details/gygdiqaii.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gexibgvpf.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gkvsgwkce.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gxoduklhg.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gqhifftft.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gwyghnptz.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/goeddgbtu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.zdbjq.cn/Article/details/gttslbwwu.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gcjuuyabv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gnjxiiqrb.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gsebkjdpi.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqbvaleag.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/glreyllyp.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gvsczqtmr.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gklaydurn.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gyohksxlc.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/guipmkpoq.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gkuhumczz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/glwnawyho.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gwcxjpmap.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/grgsxonwx.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/guctouqkw.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gcrwilhcf.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gpkatowzu.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gdqhebyqr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gepycjiog.sHtML

[T21] Swift：遍历
来源：http://read.share.fehbvm.com/Article/details/gwbelampb.sHtML

for x in a { print(x) }
来源：http://mobile.fehbvm.com/Article/details/gtvpnrsrk.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gmzbkhsug.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gafhqpopd.sHtML


<!-- 参考信息 -->