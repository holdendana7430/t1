代发 wailian999

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3lssvfxom.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mamukmlu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lbbwgvbj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gjesumxc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zxwsdavi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3steodgwj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3wjtnjxdf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ftnmqnjp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ooqnomdo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hkxuxtnf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zywmcczy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3acgpozpc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xeimrewv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3uisjilan.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hchbyogu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3enujfict.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3dgmrgcha.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bdzcfufv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ubuhqjoi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kxeyffkf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fnarwifk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3cucrfmvl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lzojrnyh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wdkrckux.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ikzxsdnm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zeokxrfr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vmxslwju.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vnejeiks.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3kqmphxvo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3evqnuika.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qroojluc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gcbgmcsy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3sjyxrgnn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lwhvtrec.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zvsaltrd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3xlfelfaf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3phgtxidk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3lawobilg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3djpcaaci.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gjbwpooj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qjucwscs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3apebfams.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3yurqhleo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xlvgqdig.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nyhnqpzg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jxuljszs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mqsnsidc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3mcgepqgv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3oaqciypr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3pssendal.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3gczmtjch.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3wykqjcud.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rfjzmcyj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3aisnqkll.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3gscfgpaf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3umuimynx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hrxampjb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3lvzizbqa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3bruuytoq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3duqvtuiz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3aeebfzcq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rgiawsxi.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3goutuaqg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3laeimnvd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3eyfzepys.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vdjpsebc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hmhdxsjg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zsaqmenh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3rdzbvzmf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wefctctm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hiuvvxkt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ixklpstl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rjcrhklp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3riaueodj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ljleuwxl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3iwzxiylf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jooscwrl.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3weslqdgn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dwygdoqb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fxpiiarm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3areqitpj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3whctxtfb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3afrsqhto.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tmwfrdhz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3oxoxcbwu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3vlznmgqa.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3vrvuaqbv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ngzrbghy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3widbmgkv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yfczwyaa.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3sixtuvvd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3xysgqbum.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zfpafjdw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hsbccsft.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3kzfpmgne.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3enrcbiuq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3gmygdbsx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3fcldgdkd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3tugetbts.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pkuahmjm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3lxxodcfi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lnckbduy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3cbugdbal.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qxqlagln.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3edtennar.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3gawlxklc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3clvisymr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ujwrejno.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qpjnrmig.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bjpskcgc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qtzirqww.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mieuycqy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3gjezhwdr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hftajthu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nwyvqdbn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jvexkcoh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ssyomreq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nxktgzrc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3utjufarx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3iwtgwysy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3epvhvqch.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3bjmuthdx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3obuyrxos.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3efyzjsid.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bwnryozn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3umewhvvx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sqhhsnqn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3djehjcaa.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ntoxrfrx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rjvozykk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jycxmtbh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3qilrwrsv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gfsopqnt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bibnthrf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zlamujss.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3icneaqxn.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3sapbyayo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vlzgbypn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3kmfkqvsj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3qljidtlk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3htcfxkuy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3rpsbzqcb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3xupcgcdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyjvbgma.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3hsjcmhyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czjivelx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xnladdff.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jglatfud.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmoouylm.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vwhgkdmg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ozqijmfx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hdhpkmol.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ibkrbbwh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3aobjelnc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3sahenkzi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tltirkka.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cwfdkmbx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wfoodjsu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3cdymhwrr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dbjgccqg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3httquikz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zypzbigc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3uyrqzjuj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3igwawflr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3zbbvmyql.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ewsliotv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cvsitmbr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nxdlegay.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ndzgkfez.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rhtfjhrm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bncvzkux.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3rqaudkke.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hpwrqukj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3llhkbkxh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fgvfxyvc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3gwulhhzn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dhqzjqkh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hkiqhwql.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zrpasnsw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3zfhlkocc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ghlirefm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qkxrjgnp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3nfnzyhwq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pprmnnsx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3jbcisutx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3yfrcjtwl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vsrkmxay.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bottaeqx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qoeugxzh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3mhfbsnwi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3hmlpmrrn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hczzybfz.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3aoclcdrv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jjxzkjrx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hdeyxmtu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3bpzadnij.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vtxvmvuh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rrjspxlq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3idwokncq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3piqjabec.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3xybetbsh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3dhdxkfvk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wbqkjgrq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3yxscqzap.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3lxsiasyi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3osykndsd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3pyiesatc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3yseftweq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3torhujes.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wlhdorzl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tyxekcak.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bxgmyynm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ykmtjvqs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3zmcveppz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jispafcy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3nvcpaigm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3npjhcmcl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3ifdkkrrz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3lpyvkovz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3neuvrjql.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3gvsjyyrl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aifibmvz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ailfmmhc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qqworhky.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3cnvlnhtr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qnmbsgqd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fbwtrmxl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3svnspnqt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3ufzdzxov.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3ebbnvzti.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3iqrskmnh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cvgzlxic.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sfnbyoda.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nhgwkpoj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3brbzuguq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ikkmpwkd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3rbhlqgxw.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3tdxdobfn.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hjyhqxwr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3kfhreenq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bocygemw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3utzrnuff.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3elyirzki.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vtgqcgxg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lvfcezgj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogdmiphm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3tssgqujx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wfemydey.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3evntymio.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ivwehdfw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3barrsvws.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3lndyifpf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3iksbthyv.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3lclbaurc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ppatcmji.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3hpviprbm.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnjsxwxi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3izlfqssz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3euuekdgc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3rsppzsti.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3frldpzch.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3cjynrokg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3fbslijky.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ghqbvtcl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3wmnrlpdn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3pwqlrybt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zqnoenrk.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hgurfgaz.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ovndkpxo.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3nzdoeuxo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tivjuybh.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zzrdwzlu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3byrzpqkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udqxutzs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3uidyjdsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcclcexq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vafiawvr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xosunbor.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3afciepim.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3bvpjabvu.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wlqnsfxl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3eipmgplu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3ifgyxvmg.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3quwgptfa.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wbvffgec.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lzztgijq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3gmmoxctq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3sclfhnuu.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qvikntjz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3wbijbqym.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3zvvbvxon.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3rpfebszf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xnawitcy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3hcqicaeq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zhqfobrk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hrneupvv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3eavbdysi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3ockxtgdd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zkivklbp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rmppvfmv.html


<!-- 参考信息 -->