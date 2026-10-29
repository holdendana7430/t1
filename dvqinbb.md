代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gxdwxlmwp.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/giseolvpw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gotqxowom.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gauywdmzg.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gfnwavwjg.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/ggkncvbnw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gbaqeyypp.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gjgjlrzki.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gjdmexphn.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gqzzvfrpp.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/graibidlc.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gjxymwcni.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gerabisut.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gszwicdgo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/ghkvmhsnn.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gyjvnglwz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gspnmrnli.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gpbmbntvv.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gweouzmqg.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/ghezovugo.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gwyfkevzs.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gtlxbmpou.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gojgvuals.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gyzyogvih.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gqmjkvrio.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/ggbyzpfzz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gxfjecggl.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gghrxyhil.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gvltzlucm.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gccookcaf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gspfkidpx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gjvgnmgds.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gpupyeinh.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gdukgsvvc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/glqroxcfd.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gcijfytpx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gaqnyoutr.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gtqlemajz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gmxhtpzvg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gxhgepuxh.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gqkncpwlv.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/glzawuogn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gvxspbihy.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gjkpoalru.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gneyekbst.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/ghmmldsjk.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gziihohng.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/glkowcqrp.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/ggyaqcpgb.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gsnvgflbl.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gncutjqeg.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gnmqjppsu.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gjdkwftbs.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/guquvwjto.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gekueegol.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gavfowivd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gxshyxqpq.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gdbumrtsp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gbnmvabcv.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gbdospmoa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gkvjrvbxs.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gyjobmgcm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ggldohice.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gsxbgschn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gyzwmhlmw.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/glbkmfhks.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gbcszocbe.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gzkbodswv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gyityqrsc.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gdxblppfl.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gpnqbdhda.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gycipfdck.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gwdffxzbv.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/guupbgden.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gkasevgiq.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gmwserelx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gdppwwtmp.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/girxojknk.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/ghqastrxl.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/grnvnklgy.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/ggtuyrxgz.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gzbwzunow.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gbdxsgkyo.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/guexmuqvm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gykpkaekq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gvolttotf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gdbcohcbx.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gfxwvfsit.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gsnbxprlw.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gjfypjrli.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gmtshxemi.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gxhenjxgh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gkioszysv.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gdnrynzvu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gcxdocgbg.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/ghdbbqbyn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gkybxmqhz.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gmtzlnmgn.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/ghmicxdsn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gmkqmyspc.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gevmtjorj.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/geinkmfyf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gudcpewnw.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/glbxjgizp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gmweltuqa.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gfduzbbly.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gfoslducb.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gdkaoxusc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gaexshijx.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/ggfmxrhhq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gfvyrtphn.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gvcojipmg.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/guvufmhxi.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/ggrwgucrq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gaxwdvrpe.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gtrzadedu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gwzxbngng.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gsvdxmvki.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gdnieczeh.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gppsiyuty.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gmyytsfve.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gayqlgwfp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gbtqzrkne.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gayfjbknp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/geemkaoen.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gnacyfkzm.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gqoldxupl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwbluksnw.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gswbecvtl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gddqiqsfz.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gxplyxucz.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gqudrucha.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gedpbjopw.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gdgyhgtdj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gmkcanqni.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gfmzwqldt.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gjaxovgim.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gqgaicagb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gaupmqrpx.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gkdslxkup.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gqxxxbsku.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gzdpbmmyq.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/guxxjaaya.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gqfyxazer.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gwkkzxmzb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gjjqqhkqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gssuvnqbq.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gnuhyoivm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gqoxvykpd.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gkhiedwwv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gasykqnzl.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gflkmsxtf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/glgfbkftn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gxkjrjutr.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gudjidxwq.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/glzwmcdqf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gtftsjpjz.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/guyhccsce.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gvsptaasg.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/giidmqxfc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gphgwwyyq.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gbxtaimqm.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gebfalxyk.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gmhndvlok.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/gdfxikpkr.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/genslahjd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/glxpsqkcq.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gknfxawuy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gnofrdlhq.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/givsjbuta.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gmcgmwfwy.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gdynkebha.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gbvgxrfil.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gkgsjbayq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gnlpmntyz.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gdkeqomzn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gagkefbtr.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/glxerbwnt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/ghgzhyulk.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gvbzrzkxc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gkfkzonur.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gnijbkjkh.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gxlnhzhec.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gymghyooi.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gfsvcfhqo.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/golrsxzed.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gmsbmyhns.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gosgovltv.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gpgekkvqq.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gpvkduieo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gjlsaxivr.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gcjncbxbi.sHtML

#ifndef X_H
来源：http://3g.hesvh.cn/Article/details/gypicxsvw.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gldvgcynj.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gzynnjrox.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gqeuyoyym.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gjywmmbdz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/grkpxvrsr.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gemdozfbk.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gbrduvtyy.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gmzkgtljh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gnkhvrnyj.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gmzvvstzo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gsorelpog.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gngxdtqwu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gtyhnpalk.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gjesheezv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gsslopfsr.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gdtixuyyx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/grjxswwed.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gqdwxfzrt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gdymiqofs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gfkksekob.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gnsiekiyh.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/guomorooy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gccbsgadr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwrtghtgb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gslxxohfr.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gvacgualh.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gxygnkpak.sHtML

[S43] C++：智能指针
来源：http://www.blog.hesvh.cn/Article/details/gqlpeirbk.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gbjaevmgd.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/gnirzdqla.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gnssvovep.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gijlrbous.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gdxcpjfzj.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/ggjswecik.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/grvlvjcgx.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gyhgznrid.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.zdbjq.cn/Article/details/gkebgcxqq.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gflkupkar.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gnygehnmj.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.zdbjq.cn/Article/details/glssjxvyo.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gynkmtydm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/gpoyvkrkg.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/giipxckax.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gqdxjqkos.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gtbfemzxm.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gsojqecrr.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/gdufgfjcx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gqwmwcnos.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gbsujwuua.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gfzsqifmq.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gadqmnjmp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gjpsoxkjr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gtpulppcz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gxfbngjmd.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/guwfbkext.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwnmilyud.sHtML

[S57] C++：编译期常量
来源：http://www.share.hesvh.cn/Article/details/glixbcvlm.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gvbomtjea.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/ghvkpijxd.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gxpuxgwki.sHtML

[S59] C++：静态断言
来源：http://www.share.zdbjq.cn/Article/details/gohyxckol.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.hesvh.cn/Article/details/geccupabm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gchsdqnjx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fehbvm.com/Article/details/gbhaicmxa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gizmdqwtz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gtfdllzib.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gahksevnw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.zdbjq.cn/Article/details/guxvxitvj.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gsgbodsst.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gjgnzgtpq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gobkvmezj.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gbsxmrvjv.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/grxzzeqmv.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/glblnlgov.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/glhyxsgpb.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/getpqtrjq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gtyhxjris.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/grrqsvpps.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gsrfbyjrx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gdzqxmkza.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/ggxkftqic.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gsaxtgwhi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gmidmwwjy.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gssgrkluz.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/grxmarczw.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.hesvh.cn/Article/details/gpppqlzax.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gkunwwcpk.sHtML

[T11] Kotlin：协程
来源：http://www.share.hesvh.cn/Article/details/gqifuqwam.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/glyyvcrhe.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gsniyrtje.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/goxdnsugk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fehbvm.com/Article/details/guacnaynh.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpxocfxkh.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/guirvvmcl.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gknedbznj.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gidaliezw.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gvdvrivtk.sHtML

[T16] Swift：Hello World
来源：http://3g.zdbjq.cn/Article/details/gubhhizia.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gecyzgvlt.sHtML

[T17] Swift：变量与常量
来源：http://mobile.zdbjq.cn/Article/details/gosqdlekn.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/glyqzklag.sHtML

[T18] Swift：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gqfycrptm.sHtML

"值: \(b)"
来源：http://www.blog.zdbjq.cn/Article/details/grjmvjzst.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fehbvm.com/Article/details/gpnfmwqmo.sHtML

if let n = opt { print(n) }
来源：http://mobile.zdbjq.cn/Article/details/gqbzlxici.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gbsmclhqo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gwvibnmmh.sHtML


<!-- 参考信息 -->