代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cdnleiting.top/gtewzdslwo.html

[R16] until 等待条件
来源：http://hz.xziqi.cn/gtuqvkoztm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fzhhl.top/gtiydiwazk.html

[R17] 数组定义与取值
来源：http://hz.shzxlz.cn/gtwsehlefw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhaomingkeji.xyz/gtrtksgalp.html

[R18] 遍历数组
来源：http://hz.gogol.net.cn/gtfsxeligx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhaomingkeji.xyz/gtnqtbnrrp.html

[R19] 数组长度
来源：http://hz.jinghuilouyu.cn/gtsymexemg.html

echo "${#arr[@]}"
来源：http://hz.dashuyun.cn/gtghxpvhzj.html

[R20] 关联数组（字典）
来源：http://hz.yj202588.top/gtphvafwnj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.quarkkingdee.top/gtsdohwczg.html

[R21] 字符串长度
来源：http://hz.nwbrower.top/gtkjnuelfh.html

echo "${#s}"
来源：http://hz.xuetiantiany.cn/gtwtynhbwe.html

[R22] 截取子串
来源：http://hz.nwbrower.top/gtzptecnaz.html

echo "${s:0:5}"
来源：http://hz.hnxiangtu.top/gtqgdovmmg.html

[R23] 字符串替换
来源：http://hz.dianchejie.cn/gtpfowrzhf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aizwys.cn/gtlauragjl.html

[R24] 大小写转换
来源：http://hz.daxiang520.top/gtgkibbkgt.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.316326.xyz/gtlzepkxrc.html

[R25] 去后缀 / 去前缀
来源：http://hz.quarkkingdee.top/gtxiswlhfm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guowangkeji.top/gtwwlbqeab.html

[R26] 命令替换
来源：http://hz.zhiwuduotai.top/gtxtwgszya.html

now=$(date +%F); echo "$now"
来源：http://hz.pengpengdd.cyou/gteqewuqll.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gtxxxkwown.html

echo $((1 + 2 * 3))
来源：http://hz.hammf.cn/gteekybgdx.html

[R28] 浮点运算
来源：http://hz.nanxuanxn.top/gtadwlgumz.html

echo "scale=2; 10/3" | bc
来源：http://hz.snrcjt.cn/gtmiekobyr.html

[R29] 定义函数
来源：http://hz.bjfxy.top/gtsofsqabz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shangyingyoupin.top/gtzbwrfpzo.html

[R30] 函数返回状态码
来源：http://hz.vqdsnc.cn/gtcuiscjpw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtfoqecdyo.html

[R31] 局部变量
来源：http://hz.tanke756.top/gtwirgkjrc.html

f() { local x=1; echo "$x"; }
来源：http://hz.sweek.top/gtevvpmdor.html

[R32] 参数个数校验
来源：http://hz.hnxiangtu.top/gtqppzbvup.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yangfankeji.com/gtodwqdwbv.html

[R33] 捕获错误并提示行号
来源：http://hz.yanxiufei.cn/gttgujmnca.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yuxming.cn/gtlufxmukd.html

[R34] 退出时清理
来源：http://hz.cashguo.top/gthkyrxofy.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.havefunace.top/gtmcbrzbof.html

[R35] 后台执行并等待
来源：http://hz.havefunace.top/gthxydzlhc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xingfuxueyuan.xyz/gtnucqpmhu.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtlaywctxf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhongyouzk.top/gtefzmhkkr.html

[R37] 把输出赋给变量
来源：http://hz.sweek.top/gtqzwgkmcy.html

files=$(ls -1)
来源：http://hz.fzhhl.top/gthlgyrgsf.html

[R38] 管道串联
来源：http://hz.kuanghao11.cn/gtbfcsksbk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.c1oappe.top/gtjzlkuejg.html

[R39] 重定向标准输出与错误
来源：http://hz.xylfe.cn/gtupqiqvqm.html

cmd > out.log 2>&1
来源：http://hz.hongshengwenyu.top/gtboazwxcp.html

[R40] 追加写日志
来源：http://hz.9152youxi.cn/gtwisdmskv.html

echo "log" >> out.log
来源：http://hz.ydjk.org.cn/gtavcmhnti.html

[R41] 丢弃输出
来源：http://hz.chenzaomai.com/gttayxbcdq.html

cmd >/dev/null 2>&1
来源：http://hz.yvedp.cn/gtvnpzvaog.html

[R42] 输入重定向
来源：http://hz.hnxiangtu.top/gtjedtvqce.html

wc -l < a.txt
来源：http://hz.tanke756.top/gthbrhyabi.html

[R43] 按名字查找文件
来源：http://hz.hysaishi.cn/gtbmqckdvv.html

find . -name "*.log" -type f
来源：http://hz.shuidangran.top/gtlgzlsrqc.html

[R44] 按修改时间查找
来源：http://hz.zhixingplan.top/gtzqwrpqod.html

find . -mtime -7 -type f
来源：http://hz.zhixingplan.top/gtfyvpnjxa.html

[R45] 批量删除
来源：http://hz.ppjwa.cn/gtkhfltert.html

find . -name "*.tmp" -delete
来源：http://hz.wangshuangyany.cn/gtpqyvdzus.html

[R46] 递归替换文件内容
来源：http://hz.hysaishi.cn/gtkvgxznzl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gtpnlowjwh.html

[R47] sed 单行替换
来源：http://hz.vqdsnc.cn/gtnibrruxt.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xziqi.cn/gtzyumdotj.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtstiiapob.html

awk '{print $1, $3}' a.txt
来源：http://hz.jianghu66.top/gthstlazda.html

[R49] awk 带条件
来源：http://hz.vqdsnc.cn/gtcncwkxkf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhijiandao.cn/gtlmezeqha.html

[R50] awk 求和
来源：http://hz.daxiang520.top/gtwyxdyrrc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenlongwang.top/gtcbjqeaiq.html

[R51] 排序去重取前几
来源：http://hz.sufxvd.cn/gtopaawrtw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.daria6918.cn/gtdpjgofxt.html

[R52] 统计行数
来源：http://hz.jinghuilouyu.cn/gtfokymkcn.html

wc -l a.txt
来源：http://hz.dianchejie.cn/gtxdjafyap.html

[R53] 查看文件头与实时尾
来源：http://hz.guowangkeji.top/gtfvtcnkvy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gotoacloud.top/gtuzponwrb.html

[R54] 比较两个文件
来源：http://hz.jianghu66.top/gtzaafkwop.html

diff a.txt b.txt
来源：http://hz.gaohongyu789.top/gtjidrizlb.html

[R55] 压缩与解压
来源：http://hz.yangfankeji.com/gtqrgmitbw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj202588.top/gtrydhedxw.html

[R56] 远程拷贝
来源：http://hz.ybcxt.top/gtspleqoai.html

scp file user@host:/path/
来源：http://hz.yvedp.cn/gthsjogbox.html

[R57] 远程执行命令
来源：http://hz.dianchejie.cn/gtrpwdznxw.html

ssh user@host 'uptime'
来源：http://hz.ydzc1.top/gtwgnztkdg.html

[R58] 下载文件
来源：http://hz.sxryk.cn/gtisbtnpgv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xylfe.cn/gthdvtxaux.html

[R59] 发 POST JSON
来源：http://hz.sweek.top/gtdpesqtbd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xziqi.cn/gtifricmwu.html

[R60] 只看 HTTP 状态码
来源：http://hz.gotoacloud.top/gtftfmrjvo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenzaomai.com/gtxblbpnyp.html

[R61] 磁盘占用
来源：http://hz.vqdsnc.cn/gtqxwpoxdu.html

df -h;  du -sh *
来源：http://hz.jiagoushi.top/gtcgfbdggh.html

[R62] 找最占空间的文件
来源：http://hz.fzhhl.top/gtolldzbyw.html

du -ah . | sort -rh | head -10
来源：http://hz.xingfuxueyuan.xyz/gtuiboybkw.html

[R63] 内存与进程
来源：http://hz.xinyue.icu/gtbcrjaoyq.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258.top/gttvhykfau.html

[R64] 结束进程
来源：http://hz.tianlin.xyz/gtmdvdthlh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sysykeji.top/gtjcpuxase.html

[R65] 查看端口占用
来源：http://hz.fzhhl.top/gtwlfymgij.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hongshengwenyu.top/gtlccptjwm.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtibmdqsay.html

crontab -e;  crontab -l
来源：http://hz.zhengqikj.top/gttzvvyamr.html

[R67] 生成随机十六进制串
来源：http://hz.yueranfly.top/gtrpvwkfuu.html

openssl rand -hex 16
来源：http://hz.iojbl.cn/gtjqqwkdex.html

[R68] 计算文件校验值
来源：http://hz.xylfe.cn/gthnxfsuzm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xuanzx.com/gtzhyvavgk.html

[R69] 生成随机密码
来源：http://hz.shzxlz.cn/gthuhiyrxj.html

head -c 16 /dev/urandom | base64
来源：http://hz.xziqi.cn/gtkcaaepzv.html

[R70] 时间戳与互转
来源：http://hz.jinqigfzy.top/gtbxslgdik.html

date +%s;  date -d @1700000000
来源：http://hz.andypj.xyz/gttzxhjuzj.html

[R71] 日期格式化
来源：http://hz.ydzc1.top/gthtrbmspx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuxming.cn/gtnnxhwdfk.html

[R72] 等待端口就绪
来源：http://hz.hongshengwenyu.top/gtyiatxgau.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinghuilouyu.cn/gthxrxhgnv.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtwfgibvvg.html

split -l 1000 big.log part_
来源：http://hz.wangdashe.top/gtuasckjaw.html

[R74] 批量重命名
来源：http://hz.hywenlv.cn/gtiltmjmmh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.birdmap.top/gtvosemdsf.html

[R75] 导出环境变量
来源：http://hz.jinqigufen.top/gtsqgfxhdx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hysaishi.cn/gtngokxdtp.html

[R76] 使用临时文件
来源：http://hz.yvedp.cn/gtcogkdxxy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtmyichyng.html

[R77] 读取用户输入
来源：http://hz.zhengqikj.top/gtkktofluh.html

read -rp "请输入: " ans
来源：http://hz.hywenlv.cn/gthtyajbjt.html

[R78] 交互式菜单
来源：http://hz.zycfv.cn/gtkggsqirv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gotoacloud.top/gtkbebjojd.html

[R79] 解析命令行选项
来源：http://hz.jiagoushi.top/gtmeezacmm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.vqdsnc.cn/gtirmphhps.html

[R80] 查看脚本执行耗时
来源：http://hz.jyoumei.cn/gtkxozztfp.html

time ./run.sh
来源：http://hz.zhixingplan.top/gtgbuodure.html

================================================================================
来源：http://hz.cucudq.cn/gtycudfxoq.html

S. C / C++ 专题
来源：http://hz.jinqigufen.top/gtwwrovdgv.html

================================================================================
来源：http://hz.aizwys.cn/gtyubpghfl.html

[S01] C：Hello World
来源：http://hz.hywenlv.cn/gtnjoyyemf.html

#include <stdio.h>
来源：http://hz.yongpay.top/gtorqqlnsb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zdqjudy.top/gtvtbzipfj.html

[S02] C：变量与格式化输出
来源：http://hz.chenzaomai.com/gtlbttawvd.html

int a = 10; printf("%d\n", a);
来源：http://hz.shuidangran.top/gtqpxykcdk.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtpgmndikc.html

int x; scanf("%d", &x);
来源：http://hz.nanxuanxn.top/gtmdxtnfro.html

[S04] C：字符串复制
来源：http://hz.tianlin.xyz/gtcqtywalr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhongyouzk.top/gtbewydfng.html

[S05] C：字符串长度
来源：http://hz.fzhhl.top/gtdftmqqjs.html

strlen(s)
来源：http://hz.cucudq.cn/gtrmaivkfz.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gtycdjbrqc.html

strcmp(a, b) == 0
来源：http://hz.xziqi.cn/gtwyoraifw.html

[S07] C：数组遍历求和
来源：http://hz.dashuyun.cn/gttfipizrw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj20258.top/gtplulosia.html

[S08] C：动态内存分配与释放
来源：http://hz.ehwqpu.com/gtzsuokcte.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zdqjudy.top/gtobqcryih.html

[S09] C：结构体定义与初始化
来源：http://hz.nwbrower.top/gtqkhuyriz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jiagoushi.top/gtnzioirtz.html

[S10] C：指针与解引用
来源：http://hz.xylfe.cn/gtmmcghlvx.html

int *p = &a;  *p = 5;
来源：http://hz.jinqigfzy.top/gtmzxydswe.html

[S11] C：逐行读文件
来源：http://hz.feifeiyinyue.top/gtelyawntd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuanzx.com/gtvpwhkxsz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtngdqzshs.html

fclose(f);
来源：http://hz.hongshengwenyu.top/gtefxeqyyg.html

[S12] C：写文件
来源：http://hz.tianlin.xyz/gtwoicohcu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gtqolgvokp.html

[S13] C：宏定义
来源：http://hz.jinghuilouyu.cn/gtxfidruml.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gotoacloud.top/gtfybpftee.html

[S14] C：枚举
来源：http://hz.316326.xyz/gtxtijjzsn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.quarkkingdee.top/gtyxlavpgv.html

[S15] C：类型转换
来源：http://hz.jqgfzy.top/gttndnpzeg.html

(double) a / b
来源：http://hz.ybcxt.top/gtzudzsace.html

[S16] C：位操作置位
来源：http://hz.sufxvd.cn/gtpgwnejyv.html

x |= (1 << 3);
来源：http://hz.yueranfly.top/gtyujpbgib.html

[S17] C：安全拼接字符串
来源：http://hz.9152youxi.cn/gtjhtatisa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pengpengdd.cyou/gtgkxmuzuq.html

[S18] C：命令行参数
来源：http://hz.shuidangran.top/gttcwydaqk.html

int main(int argc, char **argv)
来源：http://hz.jinqigufen.top/gtuegthtbq.html

[S19] C：快速排序
来源：http://hz.cdnleiting.top/gtzrhfptqa.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jqgfzy.top/gtkgkjjyse.html

[S20] C：二分查找
来源：http://hz.zhixingplan.top/gtxuauxrxp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtahuhtsul.html

[S21] C：字符类别判断
来源：http://hz.guowangkeji.top/gtekjdefzd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gtuzejizyb.html

[S22] C：字符串转数字
来源：http://hz.nanxinkj.top/gtlrcwnnaq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shangyingyoupin.top/gtlxwtksum.html

[S23] C：随机数
来源：http://hz.yj20258.top/gtxnlhvkhb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgufenzy.top/gtusbzeedi.html

[S24] C：获取本地时间
来源：http://hz.sufxvd.cn/gthhlwpsif.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.vqdsnc.cn/gtszmbfkev.html

[S25] C：内存拷贝
来源：http://hz.zhengqikj.top/gtucdrtxmq.html

memcpy(dst, src, n);
来源：http://hz.hywenlv.cn/gttttalzsp.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gtblzfmuhf.html

memset(a, 0, sizeof a);
来源：http://hz.shanyushiyangtech.top/gtniawuvfb.html

[S27] C：定义常量
来源：http://hz.jlsjyb.cn/gtuvmzwodr.html

const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtlpacrtir.html

[S28] C：静态变量
来源：http://hz.ivvv.top/gtoxisclaf.html

static int counter = 0;
来源：http://hz.havefunace.top/gtxzzjwrpk.html

[S29] C：变参函数
来源：http://hz.yueranfly.top/gtkghzzhdj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinyuanbaomall.cn/gtudazbyfj.html

[S30] C：头文件保护
来源：http://hz.pengpengdd.cyou/gtaoxcwcmt.html

#ifndef X_H
来源：http://hz.yuxming.cn/gtyfnfptis.html

#define X_H
来源：http://hz.zhengqikj.top/gtxorspuha.html

#endif
来源：http://hz.xuetiantiany.cn/gtsbrgknyq.html

[S31] C++：Hello World
来源：http://hz.316326.xyz/gtwhehzwnz.html

#include <iostream>
来源：http://hz.dashuyun.cn/gtzlixxwca.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gtiqghnvve.html

[S32] C++：字符串
来源：http://hz.gzhubu.top/gtqahuhtco.html

std::string s = "hi";  s += "!";
来源：http://hz.ydzc1.top/gtyyiitxvn.html

[S33] C++：vector 增删
来源：http://hz.0kj1m.cn/gtncligxml.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.9152youxi.cn/gtjtqvdwob.html

[S34] C++：遍历 vector
来源：http://hz.wangshuangyany.cn/gtluxofcqh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yanxiufei.cn/gtxqhodzjl.html

[S35] C++：map
来源：http://hz.xuanzx.com/gtccwazgvj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shanyushiyangkeji.top/gtwthcjwka.html

[S36] C++：unordered_map
来源：http://hz.tanke756.top/gtgydxbfyk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtfcyaojez.html

[S37] C++：set
来源：http://hz.hnqzz.top/gtzgoyymor.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gtlozeelst.html

[S38] C++：排序
来源：http://hz.chenlongwang.top/gtfscqjtcp.html

std::sort(v.begin(), v.end());
来源：http://hz.yueranfly.top/gtdzzfwnly.html

[S39] C++：自定义比较器排序
来源：http://hz.zhoulong.xyz/gtyurvocdw.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.sufxvd.cn/gtjqvmharn.html

[S40] C++：查找元素
来源：http://hz.cucudq.cn/gtgarjkgig.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgufenzy.top/gtarthwpmt.html

[S41] C++：类与构造函数
来源：http://hz.jqgufenzy.top/gtteolfkby.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ivvv.top/gtsqrrmwhj.html

[S42] C++：继承与虚函数
来源：http://hz.zhiwuduotai.top/gtwwbvtqha.html

class B : public Base { public: void f() override {} };
来源：http://hz.yanxiufei.cn/gtxyztylqm.html

[S43] C++：智能指针
来源：http://hz.fengsongda.top/gtnpsneggb.html

auto p = std::make_unique<int>(5);
来源：http://hz.xingfuxueyuan.xyz/gtvysjvjfs.html

[S44] C++：引用传参
来源：http://hz.yj20258.top/gtgbvnsdej.html

void inc(int &x) { ++x; }
来源：http://hz.jinqigfzy.top/gtuwwnkypi.html

[S45] C++：lambda
来源：http://hz.nanxuanxn.top/gtmwdcdmpf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuxming.cn/gtzfpkyemp.html

[S46] C++：函数模板
来源：http://hz.hnxiangtu.top/gtzgydtenc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yanxiufei.cn/gtfmtwvkbx.html

[S47] C++：结构化绑定遍历
来源：http://hz.gogol.net.cn/gtadgsozej.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.daria6918.cn/gtpwhhyxiu.html

[S48] C++：逐行读文件
来源：http://hz.zhijiandao.cn/gtxroybsms.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.haohaochexian.top/gtkrapbdvx.html

while (std::getline(in, line)) { }
来源：http://hz.tanke756.top/gtklgpdbmf.html

[S49] C++：写文件
来源：http://hz.zycfv.cn/gttfgmxucd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.quarkkingdee.top/gtttnbiajx.html

[S50] C++：格式化数字
来源：http://hz.chenzaomai.com/gtzdwjdnvr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.snrcjt.cn/gtswmlpmkb.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gttgkfkbgu.html

static_cast<double>(a) / b
来源：http://hz.sufxvd.cn/gtvgoypqlt.html

[S52] C++：const 与 noexcept
来源：http://hz.jinqigufen.top/gtgibfmcln.html

int size() const noexcept { return n_; }
来源：http://hz.jinghuilouyu.cn/gtmnzotwbu.html

[S53] C++：移动语义
来源：http://hz.yangfankeji.com/gtgkwkfuke.html

std::vector<int> w = std::move(v);
来源：http://hz.chenzaomai.com/gtojrkglbb.html

[S54] C++：异常处理
来源：http://hz.ybcxt.top/gtbnzkormw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gaohongyu789.top/gtyctcuuqq.html

[S55] C++：结构化绑定
来源：http://hz.yj20258888.top/gtxglytaks.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gaohongyu789.top/gtsklngprf.html

[S56] C++：optional
来源：http://hz.zdqjudy.top/gthefzurva.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fengsongda.top/gtqxidchxp.html

[S57] C++：编译期常量
来源：http://hz.c1oappe.top/gtcqqioihl.html

constexpr int N = 10;
来源：http://hz.redwolf501.top/gtssetvslk.html

[S58] C++：命名空间
来源：http://hz.smart0.xyz/gtlkecljts.html

namespace ns { int f() { return 1; } }
来源：http://hz.ivvv.top/gttsvjahpg.html

[S59] C++：静态断言
来源：http://hz.dianchejie.cn/gtgdyjwztv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sysykeji.top/gtdecnkajd.html

[S60] C++：遍历并删除元素
来源：http://hz.yj20258888.top/gtyxvpsnnv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj20258.top/gtpdmvraah.html

================================================================================
来源：http://hz.316326.xyz/gtkogbrspq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gttibjuaqe.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtiqvmusgt.html

[T01] Kotlin：Hello World
来源：http://hz.shuidangran.top/gttqfaowmq.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtstkzqytv.html

[T02] Kotlin：变量
来源：http://hz.fzhhl.top/gtahfehxzd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zycfv.cn/gtpbdwoeoj.html

[T03] Kotlin：字符串模板
来源：http://hz.fengsongda.top/gtkrgdqrpf.html

"值: $b"
来源：http://hz.xylfe.cn/gtazavsvev.html

[T04] Kotlin：空安全
来源：http://hz.ybcxt.top/gtykhnkyto.html

val n: String? = null;  n?.length
来源：http://hz.havefunace.top/gtvyojhbft.html

[T05] Kotlin：when 表达式
来源：http://hz.hnxiangtu.top/gtpwohvrnu.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.havefunace.top/gtsrwaltrp.html

[T06] Kotlin：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtmjhffbyn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.iojbl.cn/gtqvhqdrra.html

[T07] Kotlin：集合过滤
来源：http://hz.daxiang520.top/gtylueefpc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuanzhike.top/gtgvlkjorr.html

[T08] Kotlin：数据类
来源：http://hz.yongpay.top/gtyvtxfobi.html

data class User(val name: String, val age: Int)
来源：http://hz.9152youxi.cn/gtlvmghssw.html

[T09] Kotlin：扩展函数
来源：http://hz.dashuyun.cn/gtdmljkbve.html

fun String.exclaim() = this + "!"
来源：http://hz.ehwqpu.com/gthcueboiw.html

[T10] Kotlin：默认参数
来源：http://hz.xuetiantiany.cn/gtihahodql.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cqqwz.cn/gtgzyqsyty.html

[T11] Kotlin：协程
来源：http://hz.guannengcc.top/gtwlwmigdc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gzhubu.top/gtdrcfegoy.html

[T12] Kotlin：解构声明
来源：http://hz.yj202588.top/gtxnezogrc.html

val (a, b) = Pair(1, 2)
来源：http://hz.smart0.xyz/gtsphhfvat.html

[T13] Kotlin：只读 Map
来源：http://hz.aibaodan.cn/gtpnfzarrl.html

val m = mapOf("a" to 1)
来源：http://hz.zycfv.cn/gtjnyfmils.html

[T14] Kotlin：循环
来源：http://hz.nanxinkj.top/gtykuaxkec.html

for (i in 1..10) println(i)
来源：http://hz.cheryme.top/gtvkytgtjo.html

[T15] Kotlin：接口
来源：http://hz.redwolf501.top/gtktymujzh.html

interface Shape { fun area(): Double }
来源：http://hz.zhijiandao.cn/gtrtcvvivx.html

[T16] Swift：Hello World
来源：http://hz.jinqigufen.top/gtxacanyox.html

print("Hello")
来源：http://hz.zycfv.cn/gtkjigagcz.html

[T17] Swift：变量与常量
来源：http://hz.xingfuxueyuan.xyz/gtoaivvecw.html

var a = 1;  let b = 2
来源：http://hz.jinyuanbaomall.cn/gtvxqgrswa.html

[T18] Swift：字符串插值
来源：http://hz.ppjwa.cn/gtmrvtcurd.html

"值: \(b)"
来源：http://hz.gzhubu.top/gtlsnqefqj.html


<!-- 参考信息 -->