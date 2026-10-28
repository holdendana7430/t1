代发 wailian999

esac
来源：http://hz.hywenlv.cn/gtcxnudplz.html

[R12] for 遍历文件
来源：http://hz.sxryk.cn/gtuynpishy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.havefunace.top/gtbjpelufy.html

[R13] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtemruvedy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jqgfzy.top/gtmaafvgdg.html

[R14] C 风格 for
来源：http://hz.nanxinkj.top/gtvcvjqbcw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xylfe.cn/gtilatrbuf.html

[R15] while 逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtddabkfzj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigfzy.top/gtipaqxfpy.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtgxpwekbm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cashguo.top/gtogqbzvyr.html

[R17] 数组定义与取值
来源：http://hz.jinqigfzy.top/gtuwipkeia.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.bjfxy.top/gtkhhqvpxt.html

[R18] 遍历数组
来源：http://hz.mhx1999.top/gtstmoccrz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.havefunace.top/gtsmqazrpf.html

[R19] 数组长度
来源：http://hz.hywenlv.cn/gtcgzuqxyl.html

echo "${#arr[@]}"
来源：http://hz.fengsongda.top/gtdxtsewxd.html

[R20] 关联数组（字典）
来源：http://hz.xziqi.cn/gtumkbhekn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.c1oappe.top/gtdeamzudk.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtqkpxttew.html

echo "${#s}"
来源：http://hz.gzhubu.top/gthbsklijp.html

[R22] 截取子串
来源：http://hz.aizwys.cn/gtnqscsyss.html

echo "${s:0:5}"
来源：http://hz.jinyuanbaomall.cn/gtlxnmdpsj.html

[R23] 字符串替换
来源：http://hz.birdmap.top/gtwuphbtvu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenjidiqi.icu/gtttspqfwq.html

[R24] 大小写转换
来源：http://hz.xinyue.icu/gtpevpflom.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jyoumei.cn/gtiyyjogqi.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgfzy.top/gtducdztpl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.316326.xyz/gtxokfnquw.html

[R26] 命令替换
来源：http://hz.ivvv.top/gtahhdjzmv.html

now=$(date +%F); echo "$now"
来源：http://hz.dianchejie.cn/gtihixcmjn.html

[R27] 算术展开
来源：http://hz.zdqjudy.top/gtvepktmqf.html

echo $((1 + 2 * 3))
来源：http://hz.andypj.xyz/gtktqdhnmz.html

[R28] 浮点运算
来源：http://hz.gzhubu.top/gtosojipuz.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxinkj.top/gtrxeeviqh.html

[R29] 定义函数
来源：http://hz.gzhubu.top/gtcoshlhhk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258.top/gtuvfsmokb.html

[R30] 函数返回状态码
来源：http://hz.gogol.net.cn/gtuleszbes.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtpdwoiikm.html

[R31] 局部变量
来源：http://hz.sufxvd.cn/gtnyzajrab.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenlongwang.top/gtowyunyvk.html

[R32] 参数个数校验
来源：http://hz.zhiwuduotai.top/gtmagmchqy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhongyouzk.top/gtefdpajvs.html

[R33] 捕获错误并提示行号
来源：http://hz.vqdsnc.cn/gtzsoxjkon.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hongshengwenyu.top/gtpvresihw.html

[R34] 退出时清理
来源：http://hz.jinqigfzy.top/gtstegzdan.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gtzjplgkyf.html

[R35] 后台执行并等待
来源：http://hz.wangshuangyany.cn/gtwlwcrdkd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sysykeji.top/gtypgfanxp.html

[R36] 并发执行多个任务
来源：http://hz.hnxiangtu.top/gtiyqfsren.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhaomingkeji.xyz/gtfvkdpdie.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtncotsqgu.html

files=$(ls -1)
来源：http://hz.yanxiufei.cn/gtnrusbefo.html

[R38] 管道串联
来源：http://hz.cucudq.cn/gtiwkckrlx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinqigfzy.top/gtyunnhjib.html

[R39] 重定向标准输出与错误
来源：http://hz.mhx1999.top/gtvufzxnpq.html

cmd > out.log 2>&1
来源：http://hz.hysaishi.cn/gtprlirtyx.html

[R40] 追加写日志
来源：http://hz.guannengcc.top/gtmjwcoclq.html

echo "log" >> out.log
来源：http://hz.chenjidiqi.icu/gtyeorucgr.html

[R41] 丢弃输出
来源：http://hz.sysykeji.top/gtkhffttlv.html

cmd >/dev/null 2>&1
来源：http://hz.cashguo.top/gtkevawljq.html

[R42] 输入重定向
来源：http://hz.yanxiufei.cn/gtqajqzzoy.html

wc -l < a.txt
来源：http://hz.jqgufenzy.top/gtxohhjgzn.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtnptngarh.html

find . -name "*.log" -type f
来源：http://hz.vqdsnc.cn/gtwygcrsla.html

[R44] 按修改时间查找
来源：http://hz.sysykeji.top/gtdzjhivxe.html

find . -mtime -7 -type f
来源：http://hz.shangyingyoupin.top/gtvhmhpdaw.html

[R45] 批量删除
来源：http://hz.bjfxy.top/gtdwliqghw.html

find . -name "*.tmp" -delete
来源：http://hz.feifeiyinyue.top/gtbbwhikwp.html

[R46] 递归替换文件内容
来源：http://hz.nanxuanxn.top/gtygcjdhzs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgufenzy.top/gtrvdwbzvi.html

[R47] sed 单行替换
来源：http://hz.sysykeji.top/gtcljppmdv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.iojbl.cn/gttqaxhtnj.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtknxdiomg.html

awk '{print $1, $3}' a.txt
来源：http://hz.pycfn.com/gtxkmfqsyt.html

[R49] awk 带条件
来源：http://hz.mhx1999.top/gtbtfxjaxk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhiwuduotai.top/gtudzicmgp.html

[R50] awk 求和
来源：http://hz.shuidangran.top/gtacgbmunf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.birdmap.top/gtamnqlnau.html

[R51] 排序去重取前几
来源：http://hz.fzhhl.top/gtcawvhdmc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhaomingkeji.xyz/gtxkzkkqhd.html

[R52] 统计行数
来源：http://hz.haohaochexian.top/gtqpqhciuh.html

wc -l a.txt
来源：http://hz.0kj1m.cn/gtjarqkxan.html

[R53] 查看文件头与实时尾
来源：http://hz.daria6918.cn/gtriqvilzf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.daxiang520.top/gtdfcrnnjy.html

[R54] 比较两个文件
来源：http://hz.gotoacloud.top/gtksoqldem.html

diff a.txt b.txt
来源：http://hz.hywenlv.cn/gtdgxsqvse.html

[R55] 压缩与解压
来源：http://hz.cdnleiting.top/gtxjlafdzs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yangfankeji.com/gtoxoxappf.html

[R56] 远程拷贝
来源：http://hz.hnqzz.top/gtasshuzbw.html

scp file user@host:/path/
来源：http://hz.hammf.cn/gtfvjsride.html

[R57] 远程执行命令
来源：http://hz.zdqjudy.top/gtsidhceqs.html

ssh user@host 'uptime'
来源：http://hz.meibo888.top/gtmsajmfhw.html

[R58] 下载文件
来源：http://hz.kuanghao11.cn/gtcyaobtrh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydzc1.top/gtdvvblyzy.html

[R59] 发 POST JSON
来源：http://hz.yuxming.cn/gtfqsabxgm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhengqikj.top/gtrpfluzaq.html

[R60] 只看 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtdqijmeou.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.guowangkeji.top/gtbepuxbtb.html

[R61] 磁盘占用
来源：http://hz.hfpthk.cn/gtvkxnzjwj.html

df -h;  du -sh *
来源：http://hz.zhixingplan.top/gtcmdxuzvt.html

[R62] 找最占空间的文件
来源：http://hz.yvedp.cn/gtbrjjotna.html

du -ah . | sort -rh | head -10
来源：http://hz.shangyingyoupin.top/gtqcxcwaxp.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gthruzjwdg.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxinkj.top/gtnyaeyecz.html

[R64] 结束进程
来源：http://hz.mhx1999.top/gtszpcllrt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhaomingkeji.xyz/gtbfdnuqza.html

[R65] 查看端口占用
来源：http://hz.chenjidiqi.icu/gtftklawmd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tanke756.top/gtyclwvlqk.html

[R66] 定时任务
来源：http://hz.zhengqikj.top/gtrzfoedkn.html

crontab -e;  crontab -l
来源：http://hz.quarkkingdee.top/gtbgchjtwo.html

[R67] 生成随机十六进制串
来源：http://hz.hammf.cn/gtfuegamzh.html

openssl rand -hex 16
来源：http://hz.52xcode.cn/gtwqwneyde.html

[R68] 计算文件校验值
来源：http://hz.jinghuilouyu.cn/gtqlszqfbf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.52xcode.cn/gtqywbbdfu.html

[R69] 生成随机密码
来源：http://hz.zycfv.cn/gtewwrwzgc.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhijiandao.cn/gtoakhakni.html

[R70] 时间戳与互转
来源：http://hz.ydzc1.top/gtcryljcob.html

date +%s;  date -d @1700000000
来源：http://hz.yongpay.top/gtpsuqkric.html

[R71] 日期格式化
来源：http://hz.havefunace.top/gtssorukzn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ivvv.top/gthnvegpdx.html

[R72] 等待端口就绪
来源：http://hz.smart0.xyz/gtslvqejxt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gtibyxgzro.html

[R73] 分割大日志
来源：http://hz.0kj1m.cn/gtywmfaedz.html

split -l 1000 big.log part_
来源：http://hz.zhiwuduotai.top/gtcheczyuw.html

[R74] 批量重命名
来源：http://hz.fzhhl.top/gtgpmlbszp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cashguo.top/gtzvfogzhc.html

[R75] 导出环境变量
来源：http://hz.ybcxt.top/gtfcsqpqzw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tian-w.cn/gtixujybmj.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtmibldjqy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtzrbsvepg.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtoagusvvj.html

read -rp "请输入: " ans
来源：http://hz.iojbl.cn/gtunfctdyc.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtpkotatsk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guannengcc.top/gtdvqndfqh.html

[R79] 解析命令行选项
来源：http://hz.jlsjyb.cn/gtmlbgjbso.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jyoumei.cn/gtteutawgs.html

[R80] 查看脚本执行耗时
来源：http://hz.xuetiantiany.cn/gtrbqjmnlo.html

time ./run.sh
来源：http://hz.wangdashe.top/gtqztgkgsl.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtroyuuwvd.html

S. C / C++ 专题
来源：http://hz.daxiang520.top/gtxsbfntoe.html

================================================================================
来源：http://hz.wangdashe.top/gtjcjpwfdk.html

[S01] C：Hello World
来源：http://hz.chenzaomai.com/gtchuncllt.html

#include <stdio.h>
来源：http://hz.andypj.xyz/gtzgxkavpl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.guannengcc.top/gtfddjkxai.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gtsdptwnwe.html

int a = 10; printf("%d\n", a);
来源：http://hz.wangdashe.top/gtxvuzqnuf.html

[S03] C：读入整数
来源：http://hz.gotoacloud.top/gtimstkqcc.html

int x; scanf("%d", &x);
来源：http://hz.tanke756.top/gtxstvzlwn.html

[S04] C：字符串复制
来源：http://hz.gzhubu.top/gtudugfqgv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ehwqpu.com/gtbkzyzkyt.html

[S05] C：字符串长度
来源：http://hz.shangyingyoupin.top/gtefdgtnys.html

strlen(s)
来源：http://hz.pengpengdd.cyou/gtyxxxtrvz.html

[S06] C：字符串比较
来源：http://hz.0kj1m.cn/gtlhpzemxp.html

strcmp(a, b) == 0
来源：http://hz.hysaishi.cn/gtndufopiz.html

[S07] C：数组遍历求和
来源：http://hz.sysykeji.top/gtehickwrv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.meibo888.top/gtqvhktvdt.html

[S08] C：动态内存分配与释放
来源：http://hz.yongpay.top/gtmxybkxmi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtqzbdvatp.html

[S09] C：结构体定义与初始化
来源：http://hz.9152youxi.cn/gtyyifmsys.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xingfuxueyuan.xyz/gtqgqsslfi.html

[S10] C：指针与解引用
来源：http://hz.smart0.xyz/gtxqzpqeuo.html

int *p = &a;  *p = 5;
来源：http://hz.wangdashe.top/gtgoakeryz.html

[S11] C：逐行读文件
来源：http://hz.birdmap.top/gtpmglrupl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gtpuasslvw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gzhubu.top/gtxdbwmlsj.html

fclose(f);
来源：http://hz.yangfankeji.com/gtnivvssvu.html

[S12] C：写文件
来源：http://hz.fzhhl.top/gtjznmzmqz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.haohaochexian.top/gtjcsmoeno.html

[S13] C：宏定义
来源：http://hz.xziqi.cn/gtstxklgdp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gzhubu.top/gtmrkrccbc.html

[S14] C：枚举
来源：http://hz.daxiang520.top/gtyxywmcay.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pengpengdd.cyou/gtvvhnomfu.html

[S15] C：类型转换
来源：http://hz.jinqigufen.top/gthpevjuur.html

(double) a / b
来源：http://hz.fengsongda.top/gtuebkxnrg.html

[S16] C：位操作置位
来源：http://hz.dashuyun.cn/gtzuqmzrik.html

x |= (1 << 3);
来源：http://hz.ydzc1.top/gtjnnsihbw.html

[S17] C：安全拼接字符串
来源：http://hz.zhongyouzk.top/gtzpvbphsd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.bjfxy.top/gtkhhrfbln.html

[S18] C：命令行参数
来源：http://hz.hnqzz.top/gtbumyonwv.html

int main(int argc, char **argv)
来源：http://hz.shangyingyoupin.top/gtsilajkdk.html

[S19] C：快速排序
来源：http://hz.ydjk.org.cn/gtwwefkpuj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtlahtkqux.html

[S20] C：二分查找
来源：http://hz.tianlin.xyz/gtnoblxqry.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtwzcxdfzk.html

[S21] C：字符类别判断
来源：http://hz.zdqjudy.top/gtfpzfmrsg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cashguo.top/gtblmdycba.html

[S22] C：字符串转数字
来源：http://hz.ivvv.top/gtevznrodq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinqigufen.top/gtdacqlose.html

[S23] C：随机数
来源：http://hz.meibo888.top/gtpznlphdg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtitebcoup.html

[S24] C：获取本地时间
来源：http://hz.chenlongwang.top/gtaqqqkfgx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jqgfzy.top/gtkmufuskp.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtqszqfdmz.html

memcpy(dst, src, n);
来源：http://hz.xziqi.cn/gtssvqiohu.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gtqlalndqm.html

memset(a, 0, sizeof a);
来源：http://hz.sweek.top/gtjzrllyne.html

[S27] C：定义常量
来源：http://hz.tian-w.cn/gtwblovcea.html

const double PI = 3.14159;
来源：http://hz.guowangkeji.top/gttnlbhzia.html

[S28] C：静态变量
来源：http://hz.yanxiufei.cn/gtghwjpvrl.html

static int counter = 0;
来源：http://hz.hnxiangtu.top/gtlvozzbib.html

[S29] C：变参函数
来源：http://hz.0kj1m.cn/gtknqolqwu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tian-w.cn/gtswfscqgm.html

[S30] C：头文件保护
来源：http://hz.jinqigfzy.top/gtuvbuygpm.html

#ifndef X_H
来源：http://hz.yvedp.cn/gtigqgsxcw.html

#define X_H
来源：http://hz.xylfe.cn/gtieswtynt.html

#endif
来源：http://hz.hnxiangtu.top/gtuwqzprgx.html

[S31] C++：Hello World
来源：http://hz.zycfv.cn/gtpdwqcbsx.html

#include <iostream>
来源：http://hz.hongshengwenyu.top/gthpproyrs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.guowangkeji.top/gtfmfwucjf.html

[S32] C++：字符串
来源：http://hz.wangdashe.top/gtmhxqqyzn.html

std::string s = "hi";  s += "!";
来源：http://hz.jlsjyb.cn/gthfbuansb.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtvscoopip.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hongshengwenyu.top/gtudsjuxun.html

[S34] C++：遍历 vector
来源：http://hz.dianchejie.cn/gtnlbvtzva.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jlsjyb.cn/gtwbwddyfy.html

[S35] C++：map
来源：http://hz.jinqigufen.top/gtezofivoc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtcpklidqt.html

[S36] C++：unordered_map
来源：http://hz.jinghuilouyu.cn/gthniufgqu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtgrhbvlhj.html

[S37] C++：set
来源：http://hz.aibaodan.cn/gthipifgkg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenzaomai.com/gtljctqgdd.html

[S38] C++：排序
来源：http://hz.0kj1m.cn/gtlwjflssm.html

std::sort(v.begin(), v.end());
来源：http://hz.yangfankeji.com/gthvrxleod.html

[S39] C++：自定义比较器排序
来源：http://hz.gogol.net.cn/gtktxbdekr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shuidangran.top/gtmcrldnpe.html

[S40] C++：查找元素
来源：http://hz.sufxvd.cn/gtevdvgjom.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sxryk.cn/gtfnjrkxec.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gttkwsbgmj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sysykeji.top/gtppnzwdjh.html

[S42] C++：继承与虚函数
来源：http://hz.52xcode.cn/gtaterhfcn.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinyuanbaomall.cn/gtcmqpcjcb.html

[S43] C++：智能指针
来源：http://hz.nwbrower.top/gtwkzitets.html

auto p = std::make_unique<int>(5);
来源：http://hz.iojbl.cn/gtzlfewqrm.html

[S44] C++：引用传参
来源：http://hz.9152youxi.cn/gtdzvpupoo.html

void inc(int &x) { ++x; }
来源：http://hz.sxryk.cn/gtqofhrugk.html

[S45] C++：lambda
来源：http://hz.iojbl.cn/gtmdilbcbr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yangfankeji.com/gtbtrbpkuu.html

[S46] C++：函数模板
来源：http://hz.cheryme.top/gtmnpmleph.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.snrcjt.cn/gtvbffjjhb.html

[S47] C++：结构化绑定遍历
来源：http://hz.cashguo.top/gthylxqhif.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.haohaochexian.top/gtbdammgvm.html

[S48] C++：逐行读文件
来源：http://hz.iojbl.cn/gtxdniwlqq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yongpay.top/gtfpmlwnhg.html

while (std::getline(in, line)) { }
来源：http://hz.hammf.cn/gtapbkrnsw.html

[S49] C++：写文件
来源：http://hz.tanke756.top/gtrokqjpro.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxuanxn.top/gtdclgssif.html

[S50] C++：格式化数字
来源：http://hz.aizwys.cn/gtpjxnalnh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yueranfly.top/gtkthivlkt.html

[S51] C++：显式类型转换
来源：http://hz.zhongyouzk.top/gtegaeezpb.html

static_cast<double>(a) / b
来源：http://hz.havefunace.top/gtjqzyjdly.html

[S52] C++：const 与 noexcept
来源：http://hz.xinyue.icu/gtbjmkhcqt.html

int size() const noexcept { return n_; }
来源：http://hz.meibo888.top/gtnbdypkde.html

[S53] C++：移动语义
来源：http://hz.dianchejie.cn/gtnzassrab.html

std::vector<int> w = std::move(v);
来源：http://hz.aizwys.cn/gtuhlmuebc.html

[S54] C++：异常处理
来源：http://hz.zycfv.cn/gtamimornk.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.cucudq.cn/gtuoqskrpb.html

[S55] C++：结构化绑定
来源：http://hz.316326.xyz/gtblgtkcdd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.guannengcc.top/gtbyrzpsyf.html

[S56] C++：optional
来源：http://hz.9152youxi.cn/gtmspifyxi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zycfv.cn/gtepaqfshs.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangtech.top/gtbpknuojz.html

constexpr int N = 10;
来源：http://hz.xylfe.cn/gtdtmzhfxp.html

[S58] C++：命名空间
来源：http://hz.birdmap.top/gtlxcfebrh.html

namespace ns { int f() { return 1; } }
来源：http://hz.hongshengwenyu.top/gtmfyoywdg.html

[S59] C++：静态断言
来源：http://hz.guannengcc.top/gtmpouxabn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.dianchejie.cn/gtjrkrevtp.html

[S60] C++：遍历并删除元素
来源：http://hz.jinyuanbaomall.cn/gtpasgnwyw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.c1oappe.top/gtgwkzlyjg.html

================================================================================
来源：http://hz.ybcxt.top/gtpbyamrtk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhaomingkeji.xyz/gtdulxayxo.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnzpfoykk.html

[T01] Kotlin：Hello World
来源：http://hz.dianchejie.cn/gtcgqwxaei.html

println("Hello")
来源：http://hz.hywenlv.cn/gtoebncxjv.html

[T02] Kotlin：变量
来源：http://hz.xinyue.icu/gtddhqksba.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.aibaodan.cn/gtokxkplvq.html

[T03] Kotlin：字符串模板
来源：http://hz.dashuyun.cn/gtzogbulhg.html

"值: $b"
来源：http://hz.kuanghao11.cn/gtlgcrfglz.html

[T04] Kotlin：空安全
来源：http://hz.ywan-chungtsiang.top/gtkapmheto.html

val n: String? = null;  n?.length
来源：http://hz.fzhhl.top/gtquzlbiez.html

[T05] Kotlin：when 表达式
来源：http://hz.chenzaomai.com/gtxavujmvi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.dianchejie.cn/gtfpauckwh.html

[T06] Kotlin：集合映射
来源：http://hz.chenzaomai.com/gtrerwwkjx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.0kj1m.cn/gtcoupeywz.html

[T07] Kotlin：集合过滤
来源：http://hz.jinghuilouyu.cn/gtegrgbedj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.316326.xyz/gttucspgbo.html

[T08] Kotlin：数据类
来源：http://hz.aibaodan.cn/gtwmotskcr.html

data class User(val name: String, val age: Int)
来源：http://hz.haohaochexian.top/gtjdyypfzj.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangkeji.top/gtxgkpkrop.html

fun String.exclaim() = this + "!"
来源：http://hz.yj20258.top/gtupfljtwq.html

[T10] Kotlin：默认参数
来源：http://hz.gogol.net.cn/gtcqrbdauz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guowangkeji.top/gtqdeinnxi.html

[T11] Kotlin：协程
来源：http://hz.aizwys.cn/gtfmqwbklm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gotoacloud.top/gtndkrjcei.html

[T12] Kotlin：解构声明
来源：http://hz.cashguo.top/gtrverlfgm.html

val (a, b) = Pair(1, 2)
来源：http://hz.ydjk.org.cn/gtzmzvtwjr.html

[T13] Kotlin：只读 Map
来源：http://hz.hywenlv.cn/gtoodnvngz.html

val m = mapOf("a" to 1)
来源：http://hz.birdmap.top/gtvgrhcbou.html

[T14] Kotlin：循环
来源：http://hz.jqgfzy.top/gtgjhjaptv.html

for (i in 1..10) println(i)
来源：http://hz.zdqjudy.top/gtdirrswef.html


<!-- 参考信息 -->