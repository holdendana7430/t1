代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ugqxoilz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dvkfytiw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fhbvtteo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iopumnxs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3dgrvdyum.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3enlogfdo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yndkccwh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mwgchzyh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lkebffvu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3eqmalges.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pxeljywt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mvvfpgqu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mnybaowv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ebmlaqmd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jjxxfftk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xmjkpalf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3pqqqkajq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iavfxiyg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3bxfsetrd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3olnhkbse.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3plownzqu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3vpnwtyao.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3yflxcpzw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fihmbctd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ewpfjqpq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ugdzluex.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3dbwujfha.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nxkyvfoq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3fhmjyxwj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3geghyuhi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3dhcvloqt.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rigldyhz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3yzpkythc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rjpnreno.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3phcwnzwf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kpdtvcld.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3npusfmkt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gkjxtflj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dhpfkxqu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lxuirbxz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3twntrlhw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3idagpvrh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3uwslpscp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ddkuenka.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmaggzfv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hvihucow.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ajubdkkp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cdgunbpo.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xoxyibvk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3qaqvydxt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3qsvaaswy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fiodamby.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ofqedpgf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3yvginlrg.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ushtahrd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3wxhnjmlv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gjqbegzm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fjijdmbg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3bgjpbsyk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nmnvnffz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bsdgtfyl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ggmumusi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3zonfrlwq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3icaojopj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zkdjzksf.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uddajhqo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ywrlwfxc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gpcnukcp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3frslpczh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lkivrmqy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nxogesvs.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3cglqymld.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3sbuzyhqp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3inpcgnin.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hjhrcoih.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kvrjiypr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3coiakihv.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxyepkgr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tzbqsenf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qkhghmhu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yhmysbwc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nvzyxtzk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cvtwlckf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xozmxqhs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mhqxzxug.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dseqtqpj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xircmzmv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ffpgsrju.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fuqffeft.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fjoxxjnr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3zhbufdxn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rvdypmyo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uddipzdz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qqnwqmoy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jzdwieiy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pcgiykbn.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3aohtqnuh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3klbtxkiy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ssbptwdj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uwomuavk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3lpppxuny.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vefetpfa.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3upmmimtm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rrusikgg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lqenfojd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3csjsoylw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3zexbzpvm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ovkkoubp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3sblftuly.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3iatzikcr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3hoqaojtz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rcjduhze.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3kwxwmlsk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ullpojkh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ttefzvpm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lnnuyiwa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3nkydjxbd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ygglvirp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3awksmlvc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mznamtcc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3uxizjece.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tlzkoloh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rwpcegfc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3rpsonbqr.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3cqmhrhbl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ktgipbal.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rlwzomma.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3yfzsdlmh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hmarsxxv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3dbasgxua.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3nqhwdoki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvcmgjgi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3spnazdoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydufvrcj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zmmhfpqy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3pcviuvbe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyqhjges.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3rfamptjj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3msrlrawq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wbuwylun.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ncrfemwm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3dltgfbbu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3tvbtikwk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bogixxnz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ahqfefnj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vqkjfyfs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hagxxnvg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3yaetouah.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rebfylxg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3saepbcqm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3eyicvwgy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gnmgchaj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3buvdbcck.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3owkurdyb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nmlijsnl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aukwnooa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3moasgdxb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rstqjvgc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rautucmx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3fldmqoho.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mkufiepy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3xynffxuw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3maxdblwj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3oxilklls.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3vsgtmagu.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3pnxitvtb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ulvasubf.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xawuhwoq.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xavsigbn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ubpsepnm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tsullqwj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qjiifnrl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3khhletck.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qexcqhme.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3aecanicc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3rrislijz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3blnvrvsb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ivdgepxx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3cooshsuw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zzyvyadd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3wkmgrhqf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3grdcqdys.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3cijceegv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yikitoqw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3tahknqgh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ipuugwcb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3htxmetah.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3uyykkufx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3jnyawczd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3haygctra.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vdamdmaa.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3dsxxzael.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mromyurc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3dfyukbwx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3hsyynuei.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ybnezaqt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3wtpfwvan.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3jqpbhlgl.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3yoaeuxlv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rflpmqfz.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3kpxtpeys.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzcppjpn.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3rmmuceaw.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3lswivjls.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uuhrjzej.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qggtqlcb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3dxinjltt.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3afrzvjkz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pasqsira.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tmmpvtyg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3idqfcaxg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3unbdhgcp.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uwsytukq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hbulfdin.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3nbvjcobr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xjnneonr.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3bpufkkgb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3iasbpnms.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3inaxowjd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3amgjeirr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oyjskhxj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3rrelhduf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3agstdzak.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3dsixtvwb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qaqkfuux.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rjwqbshi.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3rrdydcso.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3zwzhjeed.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3klbbnxuf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3yimyeohs.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3dqkklsxs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3radrvtft.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ahvvrwgm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3derzyvwm.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dlhxqvcu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3zqhtjqoe.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fctuaggx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3sbdcfqri.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3lhxebglv.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kfduioop.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sfoooluz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3tafljzzp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3pidcbrzm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3suwweovg.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnnfqfzj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zpdgojct.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3oibjgdko.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fjliwkoo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ewadhsfz.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bdajbwvh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pjntsxtw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ygawvtwl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3akblbsnz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3msymtwti.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3lfqmmerp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3uvthipsy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3qussxjne.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3aqswokbl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3usbrfivj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3clemzumt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ekxqkude.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrpgfeet.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3wsktlsrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhpwwfcs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jgnxrztp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mysugwxl.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iqnrahcy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ihclmttf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3agosjecv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hlhfwdgr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3deblsqrw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mjehgyrz.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jwcggeub.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3mtnjvsim.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3vmatdlvs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvruluxc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jktnazyq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ffxuqedf.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3afiadzij.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ebtuzcfy.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3tugdbuua.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3grprnwub.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mmeytazx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3obncnvui.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3qckrivuc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3yujbhfzn.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3wyvwzdji.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtjeaxfz.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rcdlijkr.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ibvswcfv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3vsrdgusd.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3xhwlcchx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dvqgfrpl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3iaomjvyb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gpfnibhg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fmpjikys.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3veheuwvy.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3dgzcwyvn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qazegudb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3hzvbxsyw.html


<!-- 参考信息 -->