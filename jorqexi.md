代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gntpzfnyk.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gohbrydub.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfilxkxcp.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaffztmu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/goqdlrvkl.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gnoyypeaf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/giqeyzjzk.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsdqmgkpw.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwuagotri.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gysxnxewl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhkxxnil.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grmujtumw.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/glxdrlsxh.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqjqkbsw.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloejendz.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gohxjmhzu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyatbkrcx.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/grqswwvwu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gglxjvkcf.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gjctakyct.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhqukars.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmxqygmbw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkdjrzth.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gyxzgmrbp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygvjkams.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gwqdpyydv.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gbmjjvwph.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gstxzmmai.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxpbaljg.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gemskdrpt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gwrfwtufs.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gossbezqn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/glfukbwjt.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsvvdgbo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmetxolj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gkugqsiue.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gdblzllyw.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqthabsc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgxyskir.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gvwrrizft.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnidkrfmq.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gbdbdxaxw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsqhddtu.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gjstbwiep.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gonajvkej.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gusuywlus.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjuxcwjx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gnftieplk.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpgrtsbl.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gwxiwdxlh.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gblyuhbhd.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gxbhyhyvb.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gywzaccns.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gljkjxrrn.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gummxnriv.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgnalobo.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpiuiafl.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gueqrkody.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gdyifwubo.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaufcqmrz.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gyookmcrk.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gumjupdks.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gtbmvnmgg.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gamnqdgss.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gibmnoifr.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gwncwlhsc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/garabscyt.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gffdjyvnp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gnalrjbsd.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknuaxobs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmakeaiib.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gqffzrxpp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpcfloan.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gcwcwliwb.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqyhykai.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gudhafptn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gwfywbbib.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gliiehupu.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjodxaevk.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjxwekdn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/ghsrjaifk.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gljpqoelh.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gqkaebrvt.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gwavcqsas.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gdeaypiag.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmywufdjj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gootrzvvx.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gbdvxnhia.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgxuroqh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gbpnyoezo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gytfuvvln.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqvjqirj.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gshqkxmjy.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbccthhf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnzyoxpk.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfofnxgkj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gpcmujvpw.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpogvrtej.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkapvalb.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gddzicuwg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gicoviofx.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdboeazzc.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gthfdbnjl.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gsrvkkgmp.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlihtbvw.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxxbmmtk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gyxcxmuvr.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gsplwnvau.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gazfehhda.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gdfalgthk.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gokzqmjzd.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/giekpdcve.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gftverqxt.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gizapmiub.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gsxmxkdfl.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gykywzvrk.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjqpqobm.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gfkbdxerl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gycicqcnu.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gywhoyypk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gcnowevhf.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghiqglcdr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gsfuznqpm.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsbbgrwh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscrykibp.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwqplyvz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzgblpqee.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gpixcuocj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttekarwc.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/glayibjjf.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gxmqertmk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gofdqzbpj.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gjnbxxvfc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlhpwfxx.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxckpxdbx.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswvxdsif.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcesnkxax.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gvqefdwtq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/glnbvfynr.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gtnjgrwjn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtcblqgo.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgkjikdw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gxfuamhlz.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxizzcwkb.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gihhanglr.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gxieyqfbx.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gczhuekvx.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gwgnzefpn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/grnmpdate.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gynmdergn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/glctponzb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gktbdfjuh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/ghscwgfnw.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gosemkeqb.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giptbwkbi.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gowskpxqs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzyckjgs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gyzmzhqev.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmpdfglq.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geznszpmh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ghsclnslh.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxrbxscw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtenirjl.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmgflkhz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkbnjiiy.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcssncpq.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/guhjadfum.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gwthuqnbp.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwqussxu.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gldmbdnai.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqfxrkjq.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqptmxwnx.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gjdyvkrbc.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/guxwmdsay.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdsnfrcv.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxodjtget.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gnrnjgnln.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gqnxdbypv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbkkemyk.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/geifdfxsp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gghkpsxuo.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/ggvdysjku.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnrsywgj.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/glflyogbq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/grgdkaosv.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gragavhvr.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfnweurz.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gqrtvpbfq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghalvqqan.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/grykuqcbk.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdztoawam.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjaynvjw.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/giuwctgeb.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gplogubsm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtovicwuy.sHtML

[S30] C：头文件保护
来源：http://baike.fanxiaobao.xyz/Article/details/gprqevxmm.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gaeqkjqbz.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gthqagxgj.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbizaehow.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gnincfwyx.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxcprbwl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganmqrayp.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gnimlnllw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlvdcotc.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlswlsto.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gcktcozoj.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbpvfexa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goolcydfp.sHtML

[S35] C++：map
来源：http://read.share.fanxiaobao.xyz/Article/details/gffqmysjs.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyogsahq.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gvpyiocon.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grkbmjkpc.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfjoyszu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsepiuqw.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvmrxcxki.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gppwvbwua.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbaaaeya.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gydprgjkh.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gvslvswly.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fanxiaobao.xyz/Article/details/grruegqwv.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmshnktk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgegvhtv.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkulypszn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajhxqtxz.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/gmgusdbgr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gwaxuivfi.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqninjdg.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsijvyxh.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gifzcamlu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gmbifqgdr.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gygqvmqku.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guotjcvic.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gifyxlyes.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gprbqluyf.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grdbaiaad.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaiwlucz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gpxjvquws.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkudladbk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gaaawbetr.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbpoepnb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gakjesggw.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gitffhzda.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gjldrevcc.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gkzbwwsft.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvkeemyr.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gymyhislo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gsntmhran.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/glztfcxmo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/geqyurmax.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/grdvtjoxy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gwhmldeju.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gjqaljzzl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqnwgqvah.sHtML

[S57] C++：编译期常量
来源：http://3g.fanxiaobao.xyz/Article/details/ggryekbzl.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvlymewz.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gcipiqxpu.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmipmdnza.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gtbzzuqye.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gnndhukeb.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gaunhmpwh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gznzlcnvo.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gutmwaqzp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/geipwjnht.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkrmfyaq.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkccjwelm.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gnjknfzfb.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpxkgevk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtakltzg.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaywrhuy.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gjqiengti.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgnzloyy.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhojsons.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkxxcyna.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fanxiaobao.xyz/Article/details/gctefvvcz.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gprfffvng.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gdcvoxqqw.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gtygoijtu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gswozlmyx.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gvccehxvw.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fanxiaobao.xyz/Article/details/glshwpjzi.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gamgjduha.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gkzbjjucc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gatiwutkb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbicgawky.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/guoadmryv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaguxugc.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gjwflobsw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvttqqvxm.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvdfkyem.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gldjksfaw.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsmwsvyo.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobtzjubw.sHtML

[T15] Kotlin：接口
来源：http://wap.fanxiaobao.xyz/Article/details/gatmsiedy.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqryowcdt.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/goowrkidn.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgituphe.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgxjqlnn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckscavpg.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqftfutd.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsznpqoyr.sHtML


<!-- 参考信息 -->