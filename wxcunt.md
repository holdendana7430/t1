代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sjqklidr.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tdjfcvgu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3synbhcuw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3edvwleva.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pggppldt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xbjyladk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dwmszhba.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jifyvkxv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3alxxmven.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3flvlwrko.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bktvdhir.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nbpjusoa.html

esac
来源：http://www.52xcode.cn/Article/details/gt3yjiwucdg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkrceqrf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oyjmjzvb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qzpuqaij.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3crxpqdrz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3agklejro.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kwyvpezf.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxlqmtfo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jqcrznim.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gfhqctki.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kijmrhnn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3lozydtxs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tamzhzxy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3jtmcyuky.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3lugopbxp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kpbplrog.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wjlfdoym.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oyexuumm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dwipikrr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jiiwcrjk.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wlxglhxp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wjedhbkf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jgguaxan.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ckvzzuzs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3njpknpig.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nqdpdbxk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wkdfbqjl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3eanibwtd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wmpczthy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3pyczrvkg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3vznspdcc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ldtrjirj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3lqforbze.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fbubigct.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3vjdciext.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3blbavvys.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3mkalrpsw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ddywfzby.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3rkkfmubm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3wivwdiav.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ekgcskoa.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3horkylrc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvubpixi.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3rylqdztz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3kbgdcfzx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3sopjrowv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hbzebhiw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ownnamwi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3wudpqpub.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3wvwgvqmp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3hvuxadcb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3griorxuv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uekwqnmy.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3frclzfpg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vwrlpofc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3yxsilnni.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tohiimrt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dqhuuwte.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3dehuezbj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3bkyuktit.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dxnxlmhc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hlyobaku.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ddjbzeew.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3betirmam.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3maayxoao.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ddjvutks.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gqrkvutq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zjnirqcf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bvxldage.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rosinpca.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3cosbiuum.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3tvgrwxnn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nhyoiyrc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kusdmjte.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zeelduzq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3savaaygp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3awzmpsue.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3icbjwjww.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vssehloa.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gegpsmth.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3azkzkdlu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gzoiugwq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xpkzyvmr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3utrbdzuo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wjhjzcog.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xcohtfck.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jspaydyl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3tkwoqytf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3jsuzvjte.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aofnrqtm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3dueupwae.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3monkwase.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xwongnkx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujixdmja.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3putkkeug.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ohlacyet.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nnusghnf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ptpkzoie.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3alicsggn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rqtwtrdo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3luekcnkm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjuiplgb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3lzapeeds.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3qyoijjoo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nxfmhahe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3baasqfdt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tssjsbcg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vnyggirj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wpyaitba.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3plplyrqt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ubwtxcbx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3khkxofap.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lvessets.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bchajfnk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pdpsqzwt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3itpbyvbn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ntastpln.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dorxiiqu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uxqyzpdr.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pfsejkgc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xfcotlpu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nsnshgdv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hnkcjrna.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ebkzvtxu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ureqnewr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kobtyavm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yeskdnis.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3drkxqgsa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3hbxhlrvv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxhpxvgs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yjzgeipp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3aifiejza.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kfltlkyt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3tawfbgeo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fkbksunk.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3vnsxixjt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bntzfuge.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wyvwjrbl.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3jyqmzniw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbqlgzpr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jjogeayn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhelaqwp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3spnuetva.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dzqomvqp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3gpovdzgf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ukvnndhe.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3cwbdarys.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jibfmovv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cdswrinh.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3qfwcdqge.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gtfamcnv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mhozsbvz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vgkkvnmf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tvgiieza.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3olwbpkvk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3oiryiuss.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3oxkksbqw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3logfhbxv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3urkmbruc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3zokavrrq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mtgkjusv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rhpztsbb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zqdupauf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mphtjkcj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mgciuiqj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rzrrownl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3nhfwzhdy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3uacuynuz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3gtpzysbi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3mfjscbsr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3mqatpoec.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3kclaazvi.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kwopfsxr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3pultcupl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ceyvifew.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3sasrmuiz.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xmxotyrk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3fcgbykls.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3dsxvxubj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ejffzhzz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gvyyugdl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ruvbtqxy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3lxpcqwvr.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ehoptxet.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sfhnqjdo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ofzmqefz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wseoahik.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3noykwesv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3txxwwhkh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3zvjqqpzz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nsyiworp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3sgufkudy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3nskswdtt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mwhzwkim.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3mmtverdz.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3arwuvdcq.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zydkhbqn.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3akbubcyz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nrkucahb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3ykhdaolh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3bgvtnvff.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ladbnpol.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3tuenfqpz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3gsfloxyn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3sswxbjge.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fmlmnkal.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3wtdsnrlp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yzniupba.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3lpfwccsx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntushxsi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qjrhzhce.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xsxjebjn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3cgcaeitz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rpdpqvkh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ewrbxhxo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3chfwfusd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fkwcrxzj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fcabjxku.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ybbmzyef.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3erlarjce.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3uctauoob.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eftgslbt.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tzxirxrw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3rqtxlqth.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3cgqhqpmr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3xbfmukel.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3acqbihpy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zwrmvmuz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zjdhsaeu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pxcavsig.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3abcczhll.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3wgkuiavd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3szlirubj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3msiexzqn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3msakpvrt.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3ugvxvmsc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3ziqhcdwh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3mfuizmpy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3lirmdntd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjbmozib.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wyhltkqz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqjjqyyn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jwipzsgm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3zvmgszhi.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3wvjdxwcz.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wyzkunpy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3itlahnts.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3wtfaecof.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3egibnfxv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3itoxpaon.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3hrikfqxm.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3eouaojaz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dedifdqi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3dbkmfcqk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cvuhzurp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gfdvmlxj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ouzfeskx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3asqtmbsz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gezsszgs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3piaupuzu.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahegnqab.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3jkklkgij.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wanjjasm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3halnidai.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3blznxhdz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3murphbmz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fwtqtqfd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bplwrykd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ljtoefpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3baaadgiw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vbqwsiov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aylbgkqi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xyvttdjp.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ubugamrg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xgdszjyv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ezwcjwfi.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vwnlpjuf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3liurpntd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3egawmzet.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3rniazkrk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dxtpfsel.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3ldduqwqb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3joopleje.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fqhpktlq.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fweyqjkb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kpirtxgp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ofyvgoal.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3jeshpidr.html


<!-- 参考信息 -->