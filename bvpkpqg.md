代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gjkfrezfw.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gzhaqktaz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gfawquhas.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvyyprfny.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/giiyloauj.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gfznqgvwv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gabrawqwv.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/ghhuvzkvi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gtqgutzfr.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/ghwlgqntb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gnynysdnl.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gmbdgnhnz.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gwalssjza.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gkbhyvith.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gipoigsrx.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gpvonbuvv.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gmnodydgh.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gktzdidbu.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gjbtonfhb.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gblhllfff.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gzzkvjhca.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gptmcctir.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gpltqhqhp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/ghzukzsyz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gtgyvqvly.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gvnwrrigc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/guzxpgtde.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gfqedweew.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gxyttgdua.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/grippssvj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gafdayqyo.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqqinfrxc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/glrujfwdp.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gxoebqvpj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/grhgafqfb.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gxkchbbrq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gygsnslbi.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gzuganebi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gkyklfsek.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gdxoatfsm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gebxbhmzo.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gtxrxbzro.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gdmywtgcg.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gvfigsbqp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gyxypfwjt.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/ggklhktav.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/guwoaasdv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gvlsxludr.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gjjzbmorn.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gdzrmlujb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/geeslkajs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/ghlanylsf.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/giymtvkwb.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gvkrmzgol.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gwzuwjmyz.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gzrnsljrj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gainxapuc.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gmpsqphxo.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gyjzkifzw.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gnlvrohjt.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gfxeahqcz.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gllyuyusx.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gomfwabmw.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/goawohvop.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gjvgvnatb.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gbgftqllp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/ggjgcjbhx.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gahkuwkep.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gztxpjxzv.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gzlfmlgbo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gvvpjkzlo.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gffkfmgqd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/ggzezkwsb.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gpvbbwgac.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gozwzgpqe.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gyuthrlzm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gotagoahi.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gwgssntdm.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gfvnembgx.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/ghycgrusm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/goqsnbipy.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gvkxlkien.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/ggsacrxwg.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/ggsmfnkbl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gpoigrsgk.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gzkzmnmta.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gikzeuylb.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/glhvbflha.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gyrxjksgm.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gjwfeiixa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gbvlrvcob.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gnottupcp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gsshftgxl.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gmkfbpyph.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/ghprgalis.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gwdjjfveu.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gkgwxfdox.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/ghbvbfzca.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gttattydd.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gvcighquw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gjzwqdast.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gkwoicovm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gwxmxfmwd.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gohydjmrg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gmdbngskw.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gakaprjgh.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gltpitwae.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gcusgbyax.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gidxfaigz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gmqufhocj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gmpxycypj.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gvisljpwd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gpyuqxiww.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gzfxoacgw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gpseghgfy.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gdgqfuqco.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/grnionhwu.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gckjfwyut.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ggmtkiwhy.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/ghogwpobu.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gfstjjcjf.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gzcwkhyei.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gndipiwsa.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gwpzmfjen.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gkjcbcfye.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gdkgftyzm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gkcquhoqa.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gnvaegelk.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/glpkbplvu.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gauankzkj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gzxcdyjco.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gtaummrzg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gvuwaawhd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/glvzkkvvc.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gqjwvdjzt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gguessckk.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gsjwqdqla.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfxyhzwpm.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gneaprcbb.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gayowqnri.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gddkwjdzq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gurdlrsog.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gabamsjln.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/goyseoglm.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gtppihqiy.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gbraplctg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gklmaahoa.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gxzpbvggh.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/grfctuwzg.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gbgpyltwa.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gjsfroros.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gdpsksyme.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/glnwesvfg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gmzmtjqla.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gyxrhvixn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gxmpjjzfq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gkkudttfq.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gmmywuapu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gngtpxsxn.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gpjzpcogc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gyqvpjqnb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gfnfcrihr.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gtnpwuson.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/geajncdzs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/giewntgxu.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gudvpbdrt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gzvzmluff.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gsjhcswft.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gcfvrrrpa.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfcwcqpyd.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gzedhnwwr.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gkzatcymx.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnzceqvdw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gosrqsgbo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gpaumoyoy.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gdmpeejbs.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gupifazya.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gaooovaep.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/giumsvufj.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/ggautggca.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gflqrgvls.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/grgxdycoq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gwiassfif.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/glrixrobs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gsmymrajg.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gnoghogxo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/gjxcsbqmm.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gpmsxonfo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gaieuacjg.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gvriepjmj.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/grehoogog.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gvwghwpqo.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gcilotxrb.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/glyivpazs.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gqtueigbo.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gctjlrchw.sHtML

static int counter = 0;
来源：http://www.share.zdbjq.cn/Article/details/gusaocrma.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gnvqyppss.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gkgewbnzj.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gjqqxssjk.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gminaobpp.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gqlhvyfkn.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gfcmdauen.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/grgzibnne.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gywnxfqzq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gmbrwprbh.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gzkdtfgxn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gonjlltgk.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/goetjabdg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gcxrrnkin.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gsjnjemim.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gdapuzqrf.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gvpfvfqca.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gcoslaemr.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/ggzumgtwx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsxcdfyxs.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gulovnxlb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gyqsjwagc.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gqyvivhlr.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/gpbcmajjg.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fehbvm.com/Article/details/gczxigdpr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gjjxhojpi.sHtML

[S40] C++：查找元素
来源：http://www.share.zdbjq.cn/Article/details/gbegopzhi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/grbmbvlto.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gsqjtlelm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gtpgbjsof.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/grnelxmcq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gcutvjjds.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gamztniey.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gjbwyxuth.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/gipzjmpns.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gkvkhuqin.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gwyvkkveu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gmqvzyuze.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/grkxjrhsb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtzmmdza.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/ggzwhgceg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gllbhoqgv.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gynvprnhx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gpoyveizr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gmhagpbhk.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gnxkqbdfd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gnjbzxrdj.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gbfmdzihr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjvzknzga.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gyvgjller.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gpwrchxff.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gjkwqrhrs.sHtML

int size() const noexcept { return n_; }
来源：http://3g.hesvh.cn/Article/details/gcrfelwkq.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gcswojljr.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gzxgtkety.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gfrvvqtkk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gdlmtychc.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gqalqeseb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gyhlqhrgo.sHtML

[S56] C++：optional
来源：http://baike.zdbjq.cn/Article/details/gfmnrtixm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.zdbjq.cn/Article/details/gzlbwbyim.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gozeclifh.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gltlclwmh.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gnqejwmli.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/grlbmkyhz.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gjqhumecq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gaaifsuvg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gttijhley.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/goflogabg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzezpciha.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gdfncghzp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmfamferl.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/ghijcnztg.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gbuloovhm.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gaqxrqhah.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/geakbxkem.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gstnplood.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gamubgcih.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gcovlqqac.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fehbvm.com/Article/details/gpwqhwwxl.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gxdlfixnd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.hesvh.cn/Article/details/ggunvlece.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/guimebnda.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gjwtejcus.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gyxuaefun.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.hesvh.cn/Article/details/gjydpusyg.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gklzhrpuu.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gavbpreht.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gdcypfeoj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gbqfgljbo.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gkqoddmsb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gdzliisfg.sHtML

[T11] Kotlin：协程
来源：http://read.share.fehbvm.com/Article/details/gbwkspdyw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gksctfvhr.sHtML

[T12] Kotlin：解构声明
来源：http://baike.zdbjq.cn/Article/details/gkvppvjzi.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gxobohcdf.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/gwmialumg.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/glhwxrglw.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gjbujapzo.sHtML

for (i in 1..10) println(i)
来源：http://wap.fehbvm.com/Article/details/gvirpgexy.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/guyjslhti.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fehbvm.com/Article/details/gdipuiaxr.sHtML

[T16] Swift：Hello World
来源：http://baike.fehbvm.com/Article/details/gwncxauin.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gxnfyshfb.sHtML


<!-- 参考信息 -->