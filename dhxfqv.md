代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fzhhl.top/gtcdlibltg.html

[R16] until 等待条件
来源：http://hz.cashguo.top/gtrpbdxodj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtttnbrexo.html

[R17] 数组定义与取值
来源：http://hz.xuetiantiany.cn/gtgqvjybdq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtwcqfyhcj.html

[R18] 遍历数组
来源：http://hz.nwbrower.top/gtooabickx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgufenzy.top/gtjhikwrlq.html

[R19] 数组长度
来源：http://hz.shanyushiyangtech.top/gtbqphgsxv.html

echo "${#arr[@]}"
来源：http://hz.c1oappe.top/gtveptvrgv.html

[R20] 关联数组（字典）
来源：http://hz.yongpay.top/gtycfuekwj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.52xcode.cn/gtowuxdvmr.html

[R21] 字符串长度
来源：http://hz.shuidangran.top/gtpuvyyysh.html

echo "${#s}"
来源：http://hz.cucudq.cn/gtceckfrxs.html

[R22] 截取子串
来源：http://hz.hnxiangtu.top/gtewetxtxa.html

echo "${s:0:5}"
来源：http://hz.gzhubu.top/gttpqyuido.html

[R23] 字符串替换
来源：http://hz.vqdsnc.cn/gtmzkingho.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.bjfxy.top/gtcxgfrrmb.html

[R24] 大小写转换
来源：http://hz.andypj.xyz/gtrojkltpe.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.havefunace.top/gtdpqtjdsf.html

[R25] 去后缀 / 去前缀
来源：http://hz.jiagoushi.top/gtxkbjilxm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cucudq.cn/gtirdgtrvz.html

[R26] 命令替换
来源：http://hz.zhongyouzk.top/gtvdrejmuk.html

now=$(date +%F); echo "$now"
来源：http://hz.zhongyouzk.top/gtgzqipqrb.html

[R27] 算术展开
来源：http://hz.jqgfzy.top/gtlfefruue.html

echo $((1 + 2 * 3))
来源：http://hz.yangfankeji.com/gtcncfckvt.html

[R28] 浮点运算
来源：http://hz.ydzc1.top/gtviuuwjss.html

echo "scale=2; 10/3" | bc
来源：http://hz.wangdashe.top/gtxdciubzx.html

[R29] 定义函数
来源：http://hz.cqqwz.cn/gthjllzfqn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xziqi.cn/gthenrilal.html

[R30] 函数返回状态码
来源：http://hz.shuidangran.top/gtsncmlrzt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tanke756.top/gtzvfdbzvt.html

[R31] 局部变量
来源：http://hz.shangyingyoupin.top/gtornxlvxd.html

f() { local x=1; echo "$x"; }
来源：http://hz.cashguo.top/gtwvferdst.html

[R32] 参数个数校验
来源：http://hz.andypj.xyz/gtiigdzuwn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gtnehqbxrv.html

[R33] 捕获错误并提示行号
来源：http://hz.chenjidiqi.icu/gtcabjxvaq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258.top/gtsvaufexa.html

[R34] 退出时清理
来源：http://hz.jinqigufen.top/gtmcjnlfqx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gtkxobrvhh.html

[R35] 后台执行并等待
来源：http://hz.pengpengdd.cyou/gttnehtkfc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.birdmap.top/gtnjvkgjrr.html

[R36] 并发执行多个任务
来源：http://hz.xylfe.cn/gtbmyrzsau.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgfzy.top/gtojnkyrpn.html

[R37] 把输出赋给变量
来源：http://hz.jinghuilouyu.cn/gtuggdtbfr.html

files=$(ls -1)
来源：http://hz.dashuyun.cn/gtsbrfzfmc.html

[R38] 管道串联
来源：http://hz.jinqigfzy.top/gttutdifxq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yongpay.top/gtcyyjqxfn.html

[R39] 重定向标准输出与错误
来源：http://hz.yongpay.top/gtvzsotwfh.html

cmd > out.log 2>&1
来源：http://hz.yj20258888.top/gteyaisixg.html

[R40] 追加写日志
来源：http://hz.nanxuanxn.top/gtzrfcthti.html

echo "log" >> out.log
来源：http://hz.xinyue.icu/gttrsrannr.html

[R41] 丢弃输出
来源：http://hz.iojbl.cn/gtyaofzsib.html

cmd >/dev/null 2>&1
来源：http://hz.jqgfzy.top/gtiwdyaqal.html

[R42] 输入重定向
来源：http://hz.jinghuilouyu.cn/gtlzkbanya.html

wc -l < a.txt
来源：http://hz.redwolf501.top/gtotnikvut.html

[R43] 按名字查找文件
来源：http://hz.xuetiantiany.cn/gtyhjniwad.html

find . -name "*.log" -type f
来源：http://hz.yj20258.top/gtgcxzmqud.html

[R44] 按修改时间查找
来源：http://hz.mhx1999.top/gtgkumlsmh.html

find . -mtime -7 -type f
来源：http://hz.jiagoushi.top/gtenlcemrs.html

[R45] 批量删除
来源：http://hz.shuidangran.top/gtexrllpxu.html

find . -name "*.tmp" -delete
来源：http://hz.daxiang520.top/gtpvsatmse.html

[R46] 递归替换文件内容
来源：http://hz.fengsongda.top/gtzlfzaqub.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhaomingkeji.xyz/gtrirgmsfl.html

[R47] sed 单行替换
来源：http://hz.xziqi.cn/gtrtnjzujk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cheryme.top/gtnlgwdmtu.html

[R48] awk 取指定列
来源：http://hz.hywenlv.cn/gtvyvfzhro.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxinkj.top/gtsnookfdt.html

[R49] awk 带条件
来源：http://hz.jiagoushi.top/gtxcwmowpk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jqgfzy.top/gtukcghkgs.html

[R50] awk 求和
来源：http://hz.316326.xyz/gtoilxvvrv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xylfe.cn/gtzbazhlag.html

[R51] 排序去重取前几
来源：http://hz.shuidangran.top/gtrpgzggnk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj20258888.top/gtxxxwmofo.html

[R52] 统计行数
来源：http://hz.52xcode.cn/gtafuwaxeg.html

wc -l a.txt
来源：http://hz.nwbrower.top/gtrpjexeuz.html

[R53] 查看文件头与实时尾
来源：http://hz.hnqzz.top/gtcwetmuib.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangdashe.top/gtgxtjzehb.html

[R54] 比较两个文件
来源：http://hz.yuxming.cn/gtdutglonz.html

diff a.txt b.txt
来源：http://hz.redwolf501.top/gtdgcdnqlt.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtkvauaxdb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tanke756.top/gttpqakooy.html

[R56] 远程拷贝
来源：http://hz.nwbrower.top/gtvakqywrz.html

scp file user@host:/path/
来源：http://hz.kuanghao11.cn/gtmpwmlopc.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtrtzswtpg.html

ssh user@host 'uptime'
来源：http://hz.hywenlv.cn/gtpestecec.html

[R58] 下载文件
来源：http://hz.cucudq.cn/gtfmuyommv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ybcxt.top/gtqpeiggtw.html

[R59] 发 POST JSON
来源：http://hz.sweek.top/gtwsdgxjye.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.fzhhl.top/gthtytnyrl.html

[R60] 只看 HTTP 状态码
来源：http://hz.ivvv.top/gtzwpcorvm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sysykeji.top/gtugzxboxn.html

[R61] 磁盘占用
来源：http://hz.cheryme.top/gttjbhclss.html

df -h;  du -sh *
来源：http://hz.yonumen.top/gtfpgquyef.html

[R62] 找最占空间的文件
来源：http://hz.yj202588.top/gtyuvaygkg.html

du -ah . | sort -rh | head -10
来源：http://hz.yonumen.top/gtkydsoxeh.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gtfhhjljpf.html

free -h;  ps aux | grep nginx
来源：http://hz.jinqigufen.top/gtkdpqpwpd.html

[R64] 结束进程
来源：http://hz.daxiang520.top/gtmdynswhf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yangfankeji.com/gtvdfjduil.html

[R65] 查看端口占用
来源：http://hz.hywenlv.cn/gtsjfrcvrm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydzc1.top/gtjzpwpdoy.html

[R66] 定时任务
来源：http://hz.meibo888.top/gtjpqbgbot.html

crontab -e;  crontab -l
来源：http://hz.hywenlv.cn/gtteorrpqw.html

[R67] 生成随机十六进制串
来源：http://hz.smart0.xyz/gtbrbqpugm.html

openssl rand -hex 16
来源：http://hz.chenzaomai.com/gtdohwobhu.html

[R68] 计算文件校验值
来源：http://hz.yonumen.top/gtxncuyhns.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxuanxn.top/gtudqrvdqe.html

[R69] 生成随机密码
来源：http://hz.jinqigfzy.top/gtrwzidygq.html

head -c 16 /dev/urandom | base64
来源：http://hz.iojbl.cn/gtkudjctka.html

[R70] 时间戳与互转
来源：http://hz.birdmap.top/gttyiqrokd.html

date +%s;  date -d @1700000000
来源：http://hz.xuetiantiany.cn/gtwwqbmyly.html

[R71] 日期格式化
来源：http://hz.0kj1m.cn/gtyttsplrm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuxming.cn/gtmtzxossp.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gteqoxcyjz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtlxswcyzb.html

[R73] 分割大日志
来源：http://hz.gaohongyu789.top/gtlbnprkbh.html

split -l 1000 big.log part_
来源：http://hz.zhixingplan.top/gtaopgkycm.html

[R74] 批量重命名
来源：http://hz.fzhhl.top/gtiktweapq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.316326.xyz/gtudcomjsv.html

[R75] 导出环境变量
来源：http://hz.316326.xyz/gterscqjfe.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jianghu66.top/gtbnlfhjsy.html

[R76] 使用临时文件
来源：http://hz.zhixingplan.top/gtjxhbqrlu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtphwjfyfb.html

[R77] 读取用户输入
来源：http://hz.yj202588.top/gtqgupaglr.html

read -rp "请输入: " ans
来源：http://hz.fengsongda.top/gtdnzehjhu.html

[R78] 交互式菜单
来源：http://hz.cdnleiting.top/gtlrxypaaz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yanxiufei.cn/gttxcrueaf.html

[R79] 解析命令行选项
来源：http://hz.chenzaomai.com/gtedsehica.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.feifeiyinyue.top/gttftrgjit.html

[R80] 查看脚本执行耗时
来源：http://hz.sweek.top/gtegsmmiki.html

time ./run.sh
来源：http://hz.meibo888.top/gtdnhjizjd.html

================================================================================
来源：http://hz.yongpay.top/gtkoyqhacm.html

S. C / C++ 专题
来源：http://hz.xziqi.cn/gtshjulsvi.html

================================================================================
来源：http://hz.ybcxt.top/gtqhnxhqjd.html

[S01] C：Hello World
来源：http://hz.sufxvd.cn/gtbsfwslvb.html

#include <stdio.h>
来源：http://hz.jyoumei.cn/gttmavnjin.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgfzy.top/gtioewmxjz.html

[S02] C：变量与格式化输出
来源：http://hz.redwolf501.top/gteqnhdkeq.html

int a = 10; printf("%d\n", a);
来源：http://hz.9152youxi.cn/gtxeywpbfv.html

[S03] C：读入整数
来源：http://hz.zhoulong.xyz/gtvcujgwfa.html

int x; scanf("%d", &x);
来源：http://hz.quarkkingdee.top/gtwmfizesr.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangtech.top/gtcpzyoowm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinyuanbaomall.cn/gteowtwxqp.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gtqztqsuij.html

strlen(s)
来源：http://hz.ppjwa.cn/gtqmowplzc.html

[S06] C：字符串比较
来源：http://hz.jqgfzy.top/gtrijgetvq.html

strcmp(a, b) == 0
来源：http://hz.ybcxt.top/gtfqjezzix.html

[S07] C：数组遍历求和
来源：http://hz.xylfe.cn/gtoxtfsjvf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fzhhl.top/gtrfsqoixg.html

[S08] C：动态内存分配与释放
来源：http://hz.guowangkeji.top/gthgjcghnm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtavzueuxp.html

[S09] C：结构体定义与初始化
来源：http://hz.hywenlv.cn/gtksdnorwh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cqqwz.cn/gtayxnijbk.html

[S10] C：指针与解引用
来源：http://hz.ydzc1.top/gtszadhzun.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258.top/gtsqhryzqp.html

[S11] C：逐行读文件
来源：http://hz.meibo888.top/gtpmhxjytp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xziqi.cn/gtqviilkbv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.redwolf501.top/gtomcuspfr.html

fclose(f);
来源：http://hz.kuanghao11.cn/gtfpcrzebk.html

[S12] C：写文件
来源：http://hz.yonumen.top/gtffrxxkse.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinqigufen.top/gtfdatigcy.html

[S13] C：宏定义
来源：http://hz.zhiwuduotai.top/gtlpvsqmcv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yanxiufei.cn/gtqabnbzet.html

[S14] C：枚举
来源：http://hz.hfpthk.cn/gtwjhmbiot.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dashuyun.cn/gtpkncexyz.html

[S15] C：类型转换
来源：http://hz.jqgufenzy.top/gtrocqwrzg.html

(double) a / b
来源：http://hz.aizwys.cn/gtgwgqixku.html

[S16] C：位操作置位
来源：http://hz.sweek.top/gtxagqbmul.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtbxzcylib.html

[S17] C：安全拼接字符串
来源：http://hz.hnqzz.top/gtkyxvlnqh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cqqwz.cn/gtmsgrqgah.html

[S18] C：命令行参数
来源：http://hz.guannengcc.top/gtkpkxccwn.html

int main(int argc, char **argv)
来源：http://hz.yj20258.top/gtmvcypboh.html

[S19] C：快速排序
来源：http://hz.daria6918.cn/gtisqcofiy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtxvnhygfh.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtwyrhfbcm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gtnycfhsie.html

[S21] C：字符类别判断
来源：http://hz.yuanzhike.top/gtenovnlef.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.feifeiyinyue.top/gtgxntxyee.html

[S22] C：字符串转数字
来源：http://hz.zhijiandao.cn/gticlhnqzg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shuidangran.top/gtxidpgtzv.html

[S23] C：随机数
来源：http://hz.birdmap.top/gtsxuvjluw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangdashe.top/gtcseklryn.html

[S24] C：获取本地时间
来源：http://hz.ydzc1.top/gtzuolgdtv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yueranfly.top/gtatcbiqid.html

[S25] C：内存拷贝
来源：http://hz.gaohongyu789.top/gtuqlpbjpv.html

memcpy(dst, src, n);
来源：http://hz.sxryk.cn/gtkbbpifqe.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gtuyycygyu.html

memset(a, 0, sizeof a);
来源：http://hz.snrcjt.cn/gtkiqmqjli.html

[S27] C：定义常量
来源：http://hz.yj20258888.top/gtwbbiebtc.html

const double PI = 3.14159;
来源：http://hz.shangyingyoupin.top/gtaotlnosg.html

[S28] C：静态变量
来源：http://hz.gaohongyu789.top/gtzbmjknaa.html

static int counter = 0;
来源：http://hz.zhijiandao.cn/gthffsiiqh.html

[S29] C：变参函数
来源：http://hz.zycfv.cn/gtvpjrctdj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shzxlz.cn/gteknmmpvt.html

[S30] C：头文件保护
来源：http://hz.hammf.cn/gtparmmmfx.html

#ifndef X_H
来源：http://hz.zhongyouzk.top/gtclgzfrrw.html

#define X_H
来源：http://hz.andypj.xyz/gtxlrqxoej.html

#endif
来源：http://hz.zhoulong.xyz/gtuplokofo.html

[S31] C++：Hello World
来源：http://hz.jyoumei.cn/gtfpdjgqlx.html

#include <iostream>
来源：http://hz.nanxinkj.top/gtbebqzrrc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj202588.top/gthpaoxspt.html

[S32] C++：字符串
来源：http://hz.xylfe.cn/gtiegmumyk.html

std::string s = "hi";  s += "!";
来源：http://hz.aibaodan.cn/gthfgvnngt.html

[S33] C++：vector 增删
来源：http://hz.gaohongyu789.top/gtihqilucm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.birdmap.top/gtefcqzmdl.html

[S34] C++：遍历 vector
来源：http://hz.yuxming.cn/gtkcufdojk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yj20258.top/gtuzyzwqhr.html

[S35] C++：map
来源：http://hz.yangfankeji.com/gtkfhrakgb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hywenlv.cn/gtiswmxtfw.html

[S36] C++：unordered_map
来源：http://hz.mhx1999.top/gtmntopkvz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.meibo888.top/gttmjegjoh.html

[S37] C++：set
来源：http://hz.tianlin.xyz/gtpdfearww.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jlsjyb.cn/gtjzgdiwce.html

[S38] C++：排序
来源：http://hz.gaohongyu789.top/gtpitaypzp.html

std::sort(v.begin(), v.end());
来源：http://hz.wangdashe.top/gtuzwnhflg.html

[S39] C++：自定义比较器排序
来源：http://hz.gaohongyu789.top/gtfsylfuve.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangtech.top/gttdedjndj.html

[S40] C++：查找元素
来源：http://hz.nanxuanxn.top/gtgaaeycge.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jyoumei.cn/gtqsvovfwd.html

[S41] C++：类与构造函数
来源：http://hz.hysaishi.cn/gtbufzaobz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnqzz.top/gtwhqcsqgq.html

[S42] C++：继承与虚函数
来源：http://hz.zhengqikj.top/gtukiujqkp.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258.top/gtufhbfnru.html

[S43] C++：智能指针
来源：http://hz.cdnleiting.top/gteoojybhd.html

auto p = std::make_unique<int>(5);
来源：http://hz.zycfv.cn/gtpyvznobf.html

[S44] C++：引用传参
来源：http://hz.dianchejie.cn/gtcmlyptxu.html

void inc(int &x) { ++x; }
来源：http://hz.yueranfly.top/gtsmpnxzqr.html

[S45] C++：lambda
来源：http://hz.dianchejie.cn/gtkucbbwou.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.daria6918.cn/gtdptnpwug.html

[S46] C++：函数模板
来源：http://hz.shzxlz.cn/gtdgoegipx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinghuilouyu.cn/gtlpocqbhj.html

[S47] C++：结构化绑定遍历
来源：http://hz.gogol.net.cn/gtqmjbwvui.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hywenlv.cn/gtekvroirb.html

[S48] C++：逐行读文件
来源：http://hz.ehwqpu.com/gtzqmnntkq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenzaomai.com/gtazqykiyn.html

while (std::getline(in, line)) { }
来源：http://hz.ydzc1.top/gtumkuftvg.html

[S49] C++：写文件
来源：http://hz.nanxuanxn.top/gthqahkpjs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yanxiufei.cn/gtabltvrhj.html

[S50] C++：格式化数字
来源：http://hz.hfpthk.cn/gtmzqouxxy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cdnleiting.top/gtntznypvp.html

[S51] C++：显式类型转换
来源：http://hz.yvedp.cn/gtidlyplbk.html

static_cast<double>(a) / b
来源：http://hz.shangyingyoupin.top/gtcfwrmfmf.html

[S52] C++：const 与 noexcept
来源：http://hz.jiagoushi.top/gttvzzsgip.html

int size() const noexcept { return n_; }
来源：http://hz.hfpthk.cn/gtbcxnfiij.html

[S53] C++：移动语义
来源：http://hz.ivvv.top/gtfwtikbrj.html

std::vector<int> w = std::move(v);
来源：http://hz.pycfn.com/gtoybhyjjq.html

[S54] C++：异常处理
来源：http://hz.yanxiufei.cn/gtbenykjdb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ydzc1.top/gtepmgkibv.html

[S55] C++：结构化绑定
来源：http://hz.haohaochexian.top/gtxmdeimco.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fzhhl.top/gtehsycghf.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtcfhfmajd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yuanzhike.top/gtekcaaveg.html

[S57] C++：编译期常量
来源：http://hz.zhiwuduotai.top/gtrownceph.html

constexpr int N = 10;
来源：http://hz.316326.xyz/gtmurogpqq.html

[S58] C++：命名空间
来源：http://hz.xuetiantiany.cn/gthgjhtnzd.html

namespace ns { int f() { return 1; } }
来源：http://hz.xziqi.cn/gtowzvvpyg.html

[S59] C++：静态断言
来源：http://hz.vqdsnc.cn/gtvuxdcskd.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ywan-chungtsiang.top/gtnpuigqdj.html

[S60] C++：遍历并删除元素
来源：http://hz.yonumen.top/gteoagppmj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.redwolf501.top/gtmxewfwnv.html

================================================================================
来源：http://hz.yj20258.top/gtckiqmnsq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.snrcjt.cn/gtnenemtov.html

================================================================================
来源：http://hz.guowangkeji.top/gtjtdkuiag.html

[T01] Kotlin：Hello World
来源：http://hz.cucudq.cn/gtaxzxvsjl.html

println("Hello")
来源：http://hz.pengpengdd.cyou/gtdbnzlyjf.html

[T02] Kotlin：变量
来源：http://hz.zhongyouzk.top/gthiityoaa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shzxlz.cn/gthtbapwuk.html

[T03] Kotlin：字符串模板
来源：http://hz.c1oappe.top/gtgvizwynw.html

"值: $b"
来源：http://hz.cdnleiting.top/gtpzmgeblx.html

[T04] Kotlin：空安全
来源：http://hz.yuanzhike.top/gtyaockdwh.html

val n: String? = null;  n?.length
来源：http://hz.aizwys.cn/gtlgobevbq.html

[T05] Kotlin：when 表达式
来源：http://hz.xinyue.icu/gtdrjphtgw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xinyue.icu/gtwgjucefn.html

[T06] Kotlin：集合映射
来源：http://hz.sxryk.cn/gtzulusrot.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jiagoushi.top/gtotapbzqd.html

[T07] Kotlin：集合过滤
来源：http://hz.hongshengwenyu.top/gtqefcpwad.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zycfv.cn/gtqzwpesyy.html

[T08] Kotlin：数据类
来源：http://hz.andypj.xyz/gtfchkzkvk.html

data class User(val name: String, val age: Int)
来源：http://hz.chenzaomai.com/gtykmbxzqb.html

[T09] Kotlin：扩展函数
来源：http://hz.jqgfzy.top/gthjizanzj.html

fun String.exclaim() = this + "!"
来源：http://hz.chenzaomai.com/gtwjdfaziq.html

[T10] Kotlin：默认参数
来源：http://hz.wangshuangyany.cn/gtpfzgqezu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.pengpengdd.cyou/gtzjkzcttn.html

[T11] Kotlin：协程
来源：http://hz.gaohongyu789.top/gtgienzqnq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigfzy.top/gtreblexab.html

[T12] Kotlin：解构声明
来源：http://hz.ywan-chungtsiang.top/gtmjcjsurg.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258.top/gtfqkpherk.html

[T13] Kotlin：只读 Map
来源：http://hz.ydjk.org.cn/gttvyicjcs.html

val m = mapOf("a" to 1)
来源：http://hz.cashguo.top/gtkveypbue.html

[T14] Kotlin：循环
来源：http://hz.gotoacloud.top/gtloszwxwv.html

for (i in 1..10) println(i)
来源：http://hz.guowangkeji.top/gtbabvfhbm.html

[T15] Kotlin：接口
来源：http://hz.hnqzz.top/gtofowbadb.html

interface Shape { fun area(): Double }
来源：http://hz.hysaishi.cn/gtyqbvvfqp.html

[T16] Swift：Hello World
来源：http://hz.jyoumei.cn/gtdugzvikk.html

print("Hello")
来源：http://hz.yangfankeji.com/gtnnsnxhow.html

[T17] Swift：变量与常量
来源：http://hz.zhixingplan.top/gtpfpzmelr.html

var a = 1;  let b = 2
来源：http://hz.jinqigfzy.top/gtrnkwbuea.html

[T18] Swift：字符串插值
来源：http://hz.pengpengdd.cyou/gtkqwvnicx.html

"值: \(b)"
来源：http://hz.pengpengdd.cyou/gtodgvnuxw.html


<!-- 参考信息 -->