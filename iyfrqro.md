代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsfslelm.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gtqqpvmuv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfofuhhc.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gffzcukox.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjpfnzxu.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspnaqgkn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gedfnmjyn.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gytkaeyfh.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghbhufecz.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkucghawn.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpskqgcgw.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpraktjde.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyemwzzkv.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddzmtcjb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwcsirhod.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gzoghahng.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnyusyoha.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhbsfdgu.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gcpyzelkt.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvrunpin.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gglahswqp.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gxzgwtjhr.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gxtdwvllc.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/guynfpfnu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuphckyv.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazpfrgmx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/goqoukvwh.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gandkxvry.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvxlhprq.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnouizyu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxqtgbxkr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gkltqwgsk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfcowfom.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gexvoalpy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gconkipii.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojrrorpy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gpywuoitg.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/ggibvrtzm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gieecgpxo.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmnltkki.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/grlgxijey.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsompesa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbeaswgq.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gfrglubqg.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gywjndxhe.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpriiqnha.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmvrsjnv.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjlzmifg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmacxgcmf.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gbycnswuw.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvbtvyhmc.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjbgcyqm.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/guryzbvky.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gbdlrgxoe.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqbptllh.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/giokixgvn.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gpagiprjb.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppnplgyb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gheomnibs.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gnobvxldo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjyviajf.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghssmycwv.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/guulxvtvy.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gstczjjgn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazjpbxwj.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gvaqflbcc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtypmswwp.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/grqpecmwx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gyjjimqmc.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gczpujxau.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwldenjrn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmbzyyrf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqombxtd.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghggzyijd.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gebgdnxxv.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdvqeonn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnurmwwyy.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gujpypnau.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gqkddxnhn.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfzrlnpj.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokezafsm.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gecwscmgk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gasdqgdtn.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gzntxtnqi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzlffnuo.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gokeoyhih.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gxnanzdct.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gnpheowza.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gnfezinun.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzorfctg.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqpcnfuc.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/goaeceqhm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gqxibjaof.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/geoemvhum.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayfkpetk.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gshrcopby.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gnifhnclh.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeshatsv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuqsgjes.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gluptyljx.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmhwwhsa.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gwaohyhnt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gicryvlqd.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gnnuolfxq.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/glzeahrfm.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrilitxp.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gshmaebyn.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/ggroiolaz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkkpbshs.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gxnfflyqj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhmqjglp.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gwpxjubzt.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkcidyva.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gihvzyoti.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsnknguak.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/glpekqirk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmignwnx.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsqfnril.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmjddldw.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gkvsbryla.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gtkcapzhw.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gofkwiwdg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbpdabbm.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyrwigdb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhmvivxx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjqcokuj.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gpgxowwbd.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gokeqobhp.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gjzdijotw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glqbibrog.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqmsctyg.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gsgjkpgeh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmpqhike.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gpzxrlqaa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawhwoesg.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkqyioih.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoxsqfbz.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhnuuvwd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgnfcze.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcqdtuuz.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gsplwsqgi.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/giagfiemz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxcjhjys.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gmdchvuyy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/grjipqvri.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvjkgzsh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/glcxggszd.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvqofzip.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gwshmtwmm.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsifkjao.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzjknfhv.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvyqefbn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gsqdqgyqo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmamgsgm.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjptlutd.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grckksxgx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gttnglrpe.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gryahtnya.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gvszumdyv.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gvthnhhqq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gvkyvkxvp.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gzsyaxngq.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gzocgojoj.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/grzgfupdd.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gxtkujyfw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghvqupqpv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnzcbpbh.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gniwhcslf.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guffnuvin.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbvvqovd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhufjfps.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/glzutbpwl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwditonhl.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gsjuyzvof.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gwxuaqgmr.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gmqbuqauy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpmqpdkq.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/geudxjvvc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgauvmrw.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gvziwpvts.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxafqbjo.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gvptyizkq.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gaypbzbay.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gzftxdjhz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/geddivgnb.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gkcmupmlt.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gqfirvddo.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwnlitit.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvjzydhf.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzmtlkfr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gnkiestsu.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsmfarve.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gijlqgpgb.sHtML

#define X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gputirldf.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gbekfheec.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gywjqdbdz.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzjcnshx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghrucyzvf.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gcsdpirqu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjrfjpte.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdqgxvmt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqmznipm.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/goffhibrw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhonvkrv.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gtetujyem.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgzrezig.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gocoynxtp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjqabewtk.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gbntlqozs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gnqvmuxfk.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gmukoprcu.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gxqxyviwr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gwgstxtsm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzcozzfd.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gkklhssdf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkcpwcyv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyuueane.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwremawa.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkbceggn.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrytnjqt.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gjjuszdjn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gwolnkzkv.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gzpjwsxmw.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gavhsjlxo.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gbbcppgvl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gsskpanks.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gibvkgiyb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjiitdltl.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqdupluc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdifgjuh.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpmeqiwf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gxfqsajss.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gliyfruxq.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxhqpnxvs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/ggbkmzhmv.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gdigtyxwk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gumgzargp.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gnzqcehrm.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheeugyop.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqqoqxmx.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbcjixfi.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddepnfui.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gpvrggvly.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/gkoukklwy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gdqagwmed.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ggexcbjqf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gezezjezz.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gscijpuhw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsumatqu.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gmezhcrgb.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnkruoij.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gnovplugo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvandkaas.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrjaziya.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/guoywwtcs.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkrmghfs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhmeendf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gciugaszh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/ganxefcpr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gokuhpvlx.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjpilvlm.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrlybbbg.sHtML

[T02] Kotlin：变量
来源：http://baike.fanxiaobao.xyz/Article/details/grguyffjj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/ggljclksw.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvielxpal.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsynznbks.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/ghhlkdkfq.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gqqymdxcf.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/gikbcggnb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefpffiee.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gpvudqokq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsqfsylt.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/ggrbgocab.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrlpatsh.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fanxiaobao.xyz/Article/details/gicqvrdzu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqjoqgas.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdamnadiy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gljzirkrc.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrjgykyn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjkncisw.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyraoloh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gspqpxydj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gurpbjvbw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnmsnpaa.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygemelsh.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gckfwxywm.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxnshqhx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gflpmslcx.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/geeqftfle.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjmgwhjm.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gppnjyvaa.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gsyacxtwi.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxidrjmqc.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gnjykkydt.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdxvkvuf.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnovzilfc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwkhkuit.sHtML

if let n = opt { print(n) }
来源：http://wap.fanxiaobao.xyz/Article/details/gybfhseek.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/ghysbksqh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpierqooa.sHtML


<!-- 参考信息 -->