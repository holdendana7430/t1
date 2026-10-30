代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gdgfsfmeh.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gjabzvrcs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gigbmjxon.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/grhoboayj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzfdrjtev.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gxzcrarys.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gcicbrekv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/geyxxobka.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/grrlsudmo.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gxiekyeur.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gswshqimr.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gquvklclg.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/giziezjqn.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gvgcrbtwq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/geozqeion.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gaqshtsbm.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/ggzfxtdmg.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gmghgoiql.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gksphzmaj.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gfjhgmsoa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gjfvvogdl.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gzotjlygg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gbsxzwgrj.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gqodbnwdt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gmmypkmgu.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gvzdlwcuz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gaobailpb.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gkqkfqbme.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gxkvtmfcg.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/guadrrzfm.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gcetngvpu.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/glydkjoti.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gozjhzlga.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gjpodaxbq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gcqobabhc.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/glktapjju.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gftpyuygw.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/grzutvhsk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gqppetpfh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gnbrfzknk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/glodtypfi.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gkmdcpfbm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gizwcqlnj.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/ggfbuclhv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gnibhgjtz.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/grsevtsxm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gymvrdpbs.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gnsffstkt.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gzuqdktps.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/getzrpahu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gdigdfiwp.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/guqpmctvq.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gbbqnilyj.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gmmcugled.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/geggqdgjk.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gcsnvcvac.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/ghqkixeml.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/goiducnwe.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gdyvozlns.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gmmevmcoz.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gowjzggyp.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/giuhmgebs.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/ggdqthitc.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/grufjydwh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gyxhktmhh.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gwoxcwykt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gtxlgqfui.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gjjimjcyl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmctnmkza.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gzezpnrny.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gvdpgmplq.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gunaddahi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gvjnjcoxa.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/ggwiyjbpl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ginilsuef.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gyblnvpke.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gxbhoopix.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gijeewujg.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gqfbkddrf.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gaobeujzq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gycevtoer.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/guybqmdgb.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gpzcxawio.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gyuehsmin.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gvjndgrib.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gmzxtbxma.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gajfpegob.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/ggjhrzuzn.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/grocswbfg.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/goqkhcboa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gfraebbar.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gljvziiyy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gnazbtlig.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gimcomple.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gywfhqmol.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gmthxmmrs.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gevfgkxip.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gqzascyrn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gwmndmuch.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gblvfteci.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gdnunerap.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gtczlysks.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gfdutmjdm.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gxtwbxxev.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gobdlljwv.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gnhxxdyvn.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gjxwgppvf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/ghmibhjvv.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gmfosyulp.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gvwqqxapp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/givlzhxrw.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gtyehszkc.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gbzswsawh.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/ggohudnsp.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gjdbudllz.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gsbakgasd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gvrfadvcn.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gouhhwpbx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gjmlcixmc.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gvgnbxhgf.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gvanpchhx.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gkbniubpi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/grylskagg.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gegzebbfg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gajmvfjvs.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gocvvasfk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/grdbokman.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gpczcvbul.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gqnykross.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/glvbwpnjh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/geaaglmqa.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gwbqlpiiu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gyirlwiwl.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gzerogcnr.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gvillhnta.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grnanwnee.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gapeugpjz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gngdzmszi.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gnexxrdhi.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gdeqfpzit.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/guofzqprn.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gzxtgxial.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gjdyvfrex.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/grylejbyf.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gyntffnus.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gtykjnala.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gczoyzmte.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gxtulrsfk.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gtgrugsbt.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gimrhgpky.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/ggashyedt.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gqwjxgygr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gutduhlxl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gtkvyajcj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gxuazumtb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gfjupigkq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gzacxyrte.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/godejtavk.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gzqvrdjjl.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gfsbtydqa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/grgczmlzo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gipcckjrv.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gezwlwzga.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gcaurcchm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gbwvxajgj.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gtublpxbi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gaecguqia.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gkguxawei.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gmqsapfbg.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gmsaxmhhs.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/grimtcxuq.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/guzzdezdq.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gryivojbr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/gaigmzead.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/grfmvpcvo.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gajrawbda.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/ggbcngann.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/ghufkpycn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gaxwsybji.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gjhbdwimf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gbscoksxy.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gdaigirar.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gdspcngtb.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gxiqrmpdy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gtevfmnki.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gvzuqjnth.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gcjprixvm.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwivswh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gjwyzmobo.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gkvzlqlja.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gywzreeiz.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/girjzxmwv.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gqtevlizz.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/grcrfbukg.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gygaijguv.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gtrgvvlpx.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gftmxccuz.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gxdgxbsjr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/glsbtpyqx.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gdrksjgyk.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gklvcsgpb.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gvxmdhsup.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/guyrhkjeq.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/giorzirws.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gpidgtfet.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/grukxqfrn.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gvpzrlyqc.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gjclhgrpy.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gjtxfnqvi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/giheapveh.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gckxggetr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcpbmlhk.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gxskjomdc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gtecpaldd.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gdwvejnig.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gtngamhjy.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gebteerra.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gsmokthgy.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gwlixdpzj.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/goxwjgjrb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gnvngwogm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gydvtplri.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gsqxdlzha.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gmhgnlfbs.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gbhmdiojo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gsrrqscuk.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gtilugfpu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/glqfmbyrp.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gajhwgbiy.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/glmbqjdnk.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gtslckyyc.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/govdahjyj.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gfhoncbbt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gqloyuaiu.sHtML

[S46] C++：函数模板
来源：http://blog.fehbvm.com/Article/details/gsjjjrbli.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/ggxypxxec.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gbarexmpt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gdiupxyuf.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gmjyaoeco.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gchpjrdya.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gzpppnkxt.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gvoqvertl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/godhgixrb.sHtML

[S50] C++：格式化数字
来源：http://baike.zdbjq.cn/Article/details/gfbasvqyq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gvktowaqi.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/gihqxukpz.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gkcqejity.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gvrtxrblu.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gsuywduko.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gptmvaobt.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/glajqtqwg.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gekiqiayi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gonertldq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gxwpmvthm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/goqbfqdub.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gljpxmarq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/gwybgueoh.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gxwzgkrtz.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gjueaksgd.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gtxkepibt.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gmmigwjzl.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gtcoeafbb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gksjgxmpo.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/ghdwjpros.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gugkuhcyv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjfhifdiq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/ggsombwur.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfbxtpzfr.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gowvjdekz.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/glqwarqng.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/grearlyze.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/gobatqkcv.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gpdvustky.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gpneqflgo.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gvwqpnrlj.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gbmirgouu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gyfzxihfc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/grisjpanx.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gyccawnzd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gylwyqawe.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gmbonhjor.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gpjhuegds.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gjfonaxip.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gwyqsgdvm.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gxdkbodll.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gbhmjqssw.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/ggsphoghg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/gpakorsnv.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/goifhumuc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gwxwkqiss.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gecugyift.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/guiheyrtc.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/grsukwdll.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gyydufssv.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gginvbwju.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gaukdkuqm.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gwrzvheic.sHtML

interface Shape { fun area(): Double }
来源：http://3g.zdbjq.cn/Article/details/gkhgqvled.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ganqpprnl.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gcqqayqlv.sHtML


<!-- 参考信息 -->