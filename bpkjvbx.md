代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gngzaullg.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/goiofaohy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gfscyxuur.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gxbbgbndl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gmnyyoijg.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/ghkreecce.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gerejedbv.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gtcuwxfid.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/grxpeqygg.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gpgmufone.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gjzkaftrj.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/ggeechljw.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/goavkxgpm.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gugihqigp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/genutjbzk.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gurzothni.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gslkpczbo.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/guidckeae.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gckorunkr.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gknigabzc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gkqaolbup.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gdtizwvuv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/grhuadmxb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gsgazramr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gbkmifdso.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gfotybvnb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gsgqkvyod.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gpecerjos.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/guqsodjdf.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gleeqkrtj.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gyqobeijh.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gavskqbcv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gsdquqnfj.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gyfbnpriq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/ggxddqwmt.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gjmldiwlz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghenrcrjr.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gziadjepw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gfvbepzug.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gwnxjurvw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/guymhzlur.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/gymtfahww.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gckxhhqva.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gphxjddll.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gxnlwoijd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gzjfjaqgr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gdfentzsn.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gsmusgbig.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gwvruhvjw.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gusnxhdjf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gowottavm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/grofaigji.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gfgnubgui.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gbnzceegs.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/glhlibdyb.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gbgyzfziz.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gelmcnsqw.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gsuyrxylt.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/gvibpboun.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gzofrxmck.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gtnummyky.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gxrktpwys.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gqmqbadrz.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gazkdwfxv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gcoegsogu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gbslfgnvi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gqeemeifv.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gnyxcgbyd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghlfdpiec.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gbapgtzcr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gfjijnqbb.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gnmfcodts.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gqcsaptvs.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gdfseauuh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghrupmmkr.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/geoiwaobs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/ggndldxgh.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gvivtddee.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gehdziilq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gijkbfkyz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gzfxcdscg.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gzsnfkukp.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gmsdrbkfl.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gcgxrpsjs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gfhksyhgn.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gqebdxrkb.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gfacvkihw.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gofhveyun.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gqvjsjrwa.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gzhokmtqb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gcrhcffcc.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gakfqvjmk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gghpzcxgx.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/geimtylif.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gypywfbuo.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gotavfozy.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gzexdhisq.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gagtcdxxi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gpivphlan.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/grzvubzox.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gfuoterqq.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gzkaxwnaw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gkjslwyyv.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gtamswpvi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/ginkglyxc.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gxhjgzfqc.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gcjxorjlx.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gyyvlmlbf.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gikiqjrki.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gztvmkrku.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gugrhrdxw.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gknlcueex.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gojxsloeg.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gcrfocazz.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gplksfmym.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gtnpofvqh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gffteyovn.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gtkbmnasi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gjaxptcfa.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gqaouoxbq.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gcuakybqa.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gbncpqgkg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gxulnwcsu.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ganvzpkbe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gsnboxofl.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gvfpwvoft.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gmlariuep.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gvmlznlvl.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gqxpnmslj.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/ghbwtfabx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gjtuzxbvp.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gadoeztfk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gabsvlyxe.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gvmwjufxz.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gscfvcmek.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjiiwkyqa.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gaamvokob.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwyaitgum.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gsmoirgti.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gkkikykzh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/glyhfeabt.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gyojdykbd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gyczmstaj.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gxbtuwudu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gwnuyoxlk.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gpqzocxyl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/glrqnpwzv.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gsmulcyua.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gdeszdsca.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gwulrwupa.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gzxmpxbdr.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gzvvtdoqx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gzgvvugwi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gqvufipiz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gxnyjctae.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gdcsfoynn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gezjcugdj.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gsskkeaow.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gdexzisvo.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gonhzlest.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gibtktumb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gjwtsdvfo.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gowcecbeh.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gkcelmywu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gzxuesehb.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gblnebdsc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gwovjuvgw.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gsgtrcyse.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gddfxzxbd.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gunakwork.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gkguhczxx.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gtlbcoxxx.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gmenhdayx.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/ggxzqiwvd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gjjqrwhfj.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gekodshpz.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gvfmdexbi.sHtML

[S19] C：快速排序
来源：http://blog.zdbjq.cn/Article/details/ghqpyaxom.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gyufsjsow.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gdtvtturr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gaabqsurt.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gpfpmnfoy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gdbrpmyds.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gsnvrhqgz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gwljfdpzm.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gzrnolwij.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gqsjhdgwt.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gtnpikkfn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gnonagott.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gtwmbektq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/ghuvkfykv.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ginjolhge.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gmvsoxcqy.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gpxuclcmw.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gfcyrzwfc.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/guobsjjra.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gdksovzhc.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gccxylayq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gkgdgzkoa.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gvxsducjx.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gcgbewfyg.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/glsafqsxb.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/gffmmhmms.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gtlcciroi.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gcbsyshnd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdcryunze.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gguncsktu.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gjunrcfau.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gqrafhetj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gofpeyqbp.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/ghbjjdovr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/ghdtewxwj.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gneibubqx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gbopgcinx.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gfvymflmn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gyxxxwfqd.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gleifccfc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gwhqyxjpt.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gxnvcrmxw.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gttzrwcvh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gssimaywn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gigpiieil.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/giuypbzev.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/ghujelfir.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/ghgrmbkpx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/gyqlvwrbw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gynbtsbfe.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gzsubebwy.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gynzrrwyf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gtygltfms.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gjrgwgkoh.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.zdbjq.cn/Article/details/gkudilbwh.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gnemfdkll.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gmttmvtrf.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gnvmbtcul.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gmahkaala.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gixlfgqdt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gtowsjuqj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gkvvkookm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gpicdbvez.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/ggdmxadiw.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gnuruptdg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gdzevrxwk.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gxuxmalhg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fehbvm.com/Article/details/gtccddwbt.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fehbvm.com/Article/details/gfpwyedrx.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gtifsasmo.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fehbvm.com/Article/details/gdxzuwwyz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gdvmhvwnd.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/guygrkuca.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gmqqtbnwy.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/gynbvtcyj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.zdbjq.cn/Article/details/gxoklqsfm.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gwsutmeje.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gdhiksdqs.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gfiltxjhy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gbnzideku.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gldqvfkes.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gqmawiugn.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gtszympay.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gfsbthzcn.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gjsveiqxq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gshhuhbub.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gyzrfhbqy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gntwqyayv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geqauoxhg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gglnhdtzo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpizshhsk.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdakecerj.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/grmsksrmq.sHtML

[T02] Kotlin：变量
来源：http://blog.hesvh.cn/Article/details/gzfaqsjov.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gbbfdizss.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/gaogoerbg.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gdfkxduar.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gfwrlcgos.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gtqjnhggf.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gfblowyuf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gbwxdvkhe.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gtjuaydzu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gsrwvxyxj.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gfyvoskeq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/gbwjaudco.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fehbvm.com/Article/details/glgbcdlfw.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/ghanvovgo.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gsftmveki.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fehbvm.com/Article/details/gddpqlksj.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gacbhdvjp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.zdbjq.cn/Article/details/gusgyejna.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gjukabukt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gacytniwg.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gadbnsrlo.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gggqfjbpk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gbwwxtzhq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gczwfzmog.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gffemdhkk.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/geppavpqc.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gfdpcyslx.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gchtlafyj.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpbcfrbep.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gcvnncfbf.sHtML


<!-- 参考信息 -->