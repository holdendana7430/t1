代发 wailian999

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gklxsjhdd.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gafixvdcs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gipflkcmo.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/guvskpzbu.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpglqmwie.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgdflebt.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwquivvya.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gafwmnomk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/glorxwivn.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfhkfjcv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmdtzqzj.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzsriysb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdrkagyd.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gyylqokfl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxihytnn.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gmucffzgl.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnqubpwd.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsilavls.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyugduzc.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvexowzka.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gpmqdybkz.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gwogyscer.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcbckoob.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyinorwel.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaclbtfli.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gykjulluu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsunmikd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/glcfekcxn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/grfswjtqt.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gqzlfjztx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlqlfxcm.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbrbfmmu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gmslmycbn.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfumrixz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gmqbnvnts.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvbtxtorr.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrjiucoq.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gaipjdsij.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdatycvqf.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ggucfqvhq.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/glslusebc.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrjqgcjt.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gsbbdblpe.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/ggizjnhtf.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeortlwo.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gibougyom.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsnrixikd.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqczoeonm.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gpsidtdui.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gnntiaemk.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gyyezvfqy.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhpgnjbe.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/glcigdvqx.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfirfdxj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/glrniqzkk.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunwnljfi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzrvpelou.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeprmghf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/geucnbajg.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gxwmokmnk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gzqlwqrak.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gexkwhafn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gahribevg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelxmugqo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkmiddkz.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/guwitmzmk.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gotonvfxt.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gyitohlbh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvwqirxv.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtljrnkyp.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqealigxj.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/guabghlta.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gcsdzyxir.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gkfngpagr.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gyjhqwglu.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gtizoralj.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsfmocpw.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijqycaqd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/grmhqxfxk.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkbhhfhe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwjhioql.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrglckwh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gnbewbjvq.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gusmhsasi.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gmouhqwwa.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpctwuhlc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gesmsasok.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gxkatgide.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gklmdxgok.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gtruhgzev.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmidzodbr.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gaogfklmv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gvqaradfe.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gzanndlzv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukqvefup.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gioilzmrp.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/glfnocqvq.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gddsexfff.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfelrozv.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdifvbiye.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfixgopws.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gspvoseke.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gamfwgeaz.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrlcnvjt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdbwuakx.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgieufxb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/glvzhwknr.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gyttzclir.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwfkksdq.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvtnzwuc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gplpeszys.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gdmwxymna.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjyorsnv.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiehgagb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gdgeocvby.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gtxwnzrin.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gildgyvwy.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeiajzxp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjaqflri.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuxrqbdm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkovrneqx.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxzjjffd.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gavwsjdpf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdjrwvcmp.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gpqvuvvai.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmazbfsm.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gwyiorxew.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gzeixqzcj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyymymbad.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gsanafsyu.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgqooykv.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbpjmvwm.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkharehp.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczhvleqz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkchypbt.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giizlhahy.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtnztlol.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpgqrnqn.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/guzgjtunh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyzcsyya.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbgamnsi.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gizntdyrv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevlwcagj.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhnfthhy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbketiolw.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkygaevm.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjegmrmav.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlfocvhc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gwjbdtrpa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gyywfzvcj.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfopompcr.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxcuyyzr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkeikxkf.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwmthmhp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gqhvcnqum.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gnefnptvx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gdfbsoodw.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glprfxxbi.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gxhjoadhs.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuiygkdp.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfowttedz.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gwenqkuxl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gitbpjhco.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gakkqddvv.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkyjzkwn.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysbgcege.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ghhntjzzr.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/goudoawlh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gzhybnfcv.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gywdmfoio.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gmaoejvqu.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gmojpfrlg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/grwikvgmp.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gfqealraf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gqqcvicsd.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gxybxdlqj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gissjiztn.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gdtteisxs.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbexktqq.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/guigymzrs.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjddvcjex.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/grexgbqtq.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gwyqsxqkb.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdcyyiyl.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmmkectr.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpwieqkec.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkemhzawr.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gjkddmsov.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gnobrlfvq.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/grxxrbjpl.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbldnrlj.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gouaaxltn.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gopdslhhd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjbkauhmc.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvwhdoupq.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gkmyhuznf.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkagnihee.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gxpwxntef.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gbvjhrhlc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctygrjch.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvajkalfg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzhfquyk.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuitwvda.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqojlbqhj.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocdaqrfo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzncniraa.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamubsghw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcaoajdg.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/ghjoqgkhc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtxvcwmi.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gxncrjluq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gjfnidgwc.sHtML

[S41] C++：类与构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gegzerzsy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxhjxksd.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbhisdpcf.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzenonxrn.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gyksszcng.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gqyifkwid.sHtML

[S44] C++：引用传参
来源：http://3g.fanxiaobao.xyz/Article/details/godhdtvkd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtzcudhq.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gormibxyz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gudgbvztg.sHtML

[S46] C++：函数模板
来源：http://3g.fanxiaobao.xyz/Article/details/ggvgmpruk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbvinaxx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gnudeagmd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtftlxisq.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwmbqhfey.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkolbxhd.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/goikejmvl.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghshxvjnl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdarmkrm.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gslkjiktw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gacckpuiq.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goypczhqp.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtlfdjuj.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmzmbtfi.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghgvcqlm.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gjytmfheo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdvvbulf.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gjlriwygx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fanxiaobao.xyz/Article/details/guxgzqnsv.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrwkxscg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gjtnyrbsp.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gcctfhjzc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbvfstiq.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjxzuxys.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gohwpifks.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpkefpqb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gdpftlteh.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gcuvvofhb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyutxomi.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/groyejfbd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gnfpqyqic.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzitqsupn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/glbgzgbjf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawvazuwv.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhjisaur.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgrqrpge.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfnpckny.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkofgpuw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gudkfdpwv.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gyewdempd.sHtML

[T04] Kotlin：空安全
来源：http://baike.fanxiaobao.xyz/Article/details/grmcaqsey.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gpungzngt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gfhxxmuba.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuyaqdsh.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gcviknaqp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gtdhbfabr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpjrzzav.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmipcaqwb.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdhrsdhm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskadwthn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjdsiydq.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gumlbybti.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqneiohbw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gskrvxezs.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghernbwca.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fanxiaobao.xyz/Article/details/gfzqtrqob.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gchckhxpu.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gboeliytj.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoxtcvut.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gevqcqsvj.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjceypsk.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/glqtyxblb.sHtML

[T15] Kotlin：接口
来源：http://m.share.fanxiaobao.xyz/Article/details/grbsbefim.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaowzuxf.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbbirkixj.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gaficxthf.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gsmaxgqtq.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyyupukwa.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gunasvpbq.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/ggqlccnrg.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/gboqyfaqy.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gsyovjgmg.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gwsqutldx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gpywihocq.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrqnqfzh.sHtML

for x in a { print(x) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcivsxuy.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gumfcdarq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbdechfd.sHtML


<!-- 参考信息 -->