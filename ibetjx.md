代发 wailian999

esac
来源：http://www.ydjk.org.cn/Article/details/gt2vovykuoi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dbfgujaf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2dpueteiz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2udartxza.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wbdxrtyj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vgqmsvok.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2iblpngns.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2stabjwtu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wwmrafbd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ganivcba.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gthvsnul.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2wniegoau.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wdtzbxkr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wyzrvebz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ezzcyglj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2attzdbkp.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2lvixukvj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2sontabju.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vnjyvptv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2crauhlmu.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wgdyteva.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ejqysxnp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2craougnb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tgcgkzgt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2lfjnkkcl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2tyftgttp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ucogxrbn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2oukococj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vnxcphcv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jeefjuge.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fdlpikfm.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2riqeiyxj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rxgqvgai.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2xzwhuzho.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hfpelnyd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vedkcmdz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tjaqoqor.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pmtspcro.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xolzyvid.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2emdvvuxq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjuqpwqp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2keekzfhm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwdyfkwo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2wghkpkbl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jonfikgg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qckswvaq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tauvxtta.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2teymnanw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wvgpdhbz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dpkfnxpo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2klksfsjn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ejtpjezf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2uzajbbmy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ozqgtquu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hjkywial.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wwumkhkg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yawtrtya.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2enayvtld.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2cdctisbb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2iaqowadb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wspdiqpw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2gwubshfo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fnwbkipu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2sfqwycuf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vpnprbgu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2tzednrdc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ztezsjqi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lsrypapy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2buivswhr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2rqhdsueu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2lefvqvty.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2qfbzptua.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bcttpkpq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ntkdyxfm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iljgijmu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2whbheybv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2oaxuajbi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ubucuwsl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oaxblbdh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ferazlut.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2thrltkkt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2amoggidt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cuiikbev.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2srappbtx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2binztxty.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ajwovems.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mlglavmx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ulxhozso.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ieamqtla.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vqjnirxc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2expciqgq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2objsxdbm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wwjvckvl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vecjclob.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2poexdtse.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jmmajlga.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yctzgusw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cixqbdtz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mdrcakhl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2iwnogkpu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2zuymdsib.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2joscqnac.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qsdetgmy.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xvntetgl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wpxjtyuj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cgmpyxdb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vgizkfyk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yqvhukuc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2jvtuwapr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hycgzkfc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2vpmxxhlr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lcwamnac.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cjpxoedd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fkicfoct.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2adsztlnr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vkvryblf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2lmlisqsk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qqokgixz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2tlyauspd.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eslkmxxs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2bccfziai.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mrsnioxy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lyrqwfqn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zmdgeyxz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mwaanaal.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qtlpseii.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cnunsarx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fmpzynwt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2esluwcvv.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ingdbjio.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gxsfsvda.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sneskthv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rmxoglll.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vhxprdgq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2sgwrpsdd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hnybdufb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ohesadvt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bicidavd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zltrxags.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcazbdwq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qsektxis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtceflyg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hdfcyrde.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qkcxkqqi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpmsyuxt.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2roxbnels.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2tvaooaoi.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2eyfnzuka.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vbscmttt.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2dczxaakh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dihfvoyr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fjrwxrsf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ykthqfia.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2olnqkphy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2brsfjaax.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2catmkqvd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gxugiaqi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xvkfxajk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2quyyrbnc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2cnbpcizg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2caswswsc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2datwkwak.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2guxxpqdj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2goflvxkf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cavetmsz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2wwbrwbhl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dzmkqufp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bbpeoyhi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2upswympu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ksmygder.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2xofyfxcc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rtdoxmrd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wmyxbkfb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2azczssot.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mkqisdge.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2eotzmgfb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2pvbwwnbi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2damthnzb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ycdrhujj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rlfnfkzo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wucquott.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lcpdegfh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bsxfvxvo.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yoqcgvmp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tvkhbapk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2gvlklfvq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2jqspyreu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ycorkbsw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2wtaopgum.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ojtuyxbx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qpefqdsh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rfihhksf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2uclyptgm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2osjqwlkc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ynmbiwpw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2qfbqywdz.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xzksclxi.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2pbapcnmf.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hzgqyvcf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fsugdgpj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mrtszdzd.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2qnzjxurk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zmvgqgah.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rnqbdxsn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2frxjciev.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2awrfftdr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2jyzubwwc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qfifemhl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2kdvorxpf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fljxhwel.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wofsvkms.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tlidgzwc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2thgqqafl.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ywagtfef.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2adwvntoi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2mjoclxqr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ctnolswe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2skpeingy.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2infsrfee.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2djxsmwgf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2gvxuumri.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tdulakzt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ccmdfyxz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wdakiwfj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2hlrdvxce.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dqudiwsn.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2debnqihd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vgsyvkps.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rmbasgpe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2zdedafoq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2vpqnwfto.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hwtrwjii.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2kmosxwsf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hbtyaykg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xqgxexrg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2lgolcoct.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2bftfvncc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2wjxbwixz.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zfxsoqqa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qxhptgtr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2lmygbdpe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucsawnbz.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xpwidicc.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2qakhajkt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mhziqkyl.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2adtypuhw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2zzmrbult.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2vgmweucq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uhrxvryr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2myrvpzmc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2yqkqkyui.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2accfqzfw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqawaxlh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2iyuzurvq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2huzthmka.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2joocbjen.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2byrupikx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wszennop.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dyknfqrj.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2wuhrncke.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2iohbfilg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2omljvcab.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hgemznwa.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ohcswroc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qvzhuajc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rjmrjynm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2zhnsegmn.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xbjylnhk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2aefwlvzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wscgsrcf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lkvhmoob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2floussyw.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ipnyiwbq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hxlmdivw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ukpuneym.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2lsecbxlx.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2nnmcbjsl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2wwqocnke.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2vsgnowjn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zqvreyht.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fqxvehgv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lfqvfjdc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2iyzalmdw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uvcpkomk.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bdmrcvmy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2updgioov.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2celadydd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xnffyvns.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2szatrjfz.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2inqcpjyn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2tyzoymig.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2xtfnbmgs.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2lzactbfd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2trjwgadw.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2huianyac.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofgzldeo.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jgfnnzmb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gupceamx.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ovypqlgx.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pbgjqjay.html


<!-- 参考信息 -->