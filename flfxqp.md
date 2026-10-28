代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.wangdashe.top/gtsxuaygna.html

[R16] until 等待条件
来源：http://hz.yuxming.cn/gtwoetpihy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gogol.net.cn/gtghqhjhwa.html

[R17] 数组定义与取值
来源：http://hz.jqgufenzy.top/gtxrtsfihs.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydjk.org.cn/gtyuvsditv.html

[R18] 遍历数组
来源：http://hz.guannengcc.top/gtchxjxpoj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangdashe.top/gtqyukcmur.html

[R19] 数组长度
来源：http://hz.tian-w.cn/gtftqhjysg.html

echo "${#arr[@]}"
来源：http://hz.yj20258888.top/gtogmxckhq.html

[R20] 关联数组（字典）
来源：http://hz.c1oappe.top/gtixjzfxbn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhixingplan.top/gtofgvnwjj.html

[R21] 字符串长度
来源：http://hz.yueranfly.top/gtgnvawbwr.html

echo "${#s}"
来源：http://hz.svipenyu.cn/gtjzdxgcoq.html

[R22] 截取子串
来源：http://hz.snrcjt.cn/gtnnkrqrsg.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtaoxybjql.html

[R23] 字符串替换
来源：http://hz.iojbl.cn/gtttsjdoug.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yangfankeji.com/gtlxsuulow.html

[R24] 大小写转换
来源：http://hz.yonumen.top/gthpmtiesr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yongpay.top/gtitrqzpvm.html

[R25] 去后缀 / 去前缀
来源：http://hz.andypj.xyz/gtvolpssbj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.9152youxi.cn/gtogvqjvlt.html

[R26] 命令替换
来源：http://hz.nwbrower.top/gtflxsvlaz.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtasshwvjk.html

[R27] 算术展开
来源：http://hz.sxryk.cn/gtqxntrdcn.html

echo $((1 + 2 * 3))
来源：http://hz.c1oappe.top/gtaddjgpqh.html

[R28] 浮点运算
来源：http://hz.jinqigfzy.top/gtmwmurwlb.html

echo "scale=2; 10/3" | bc
来源：http://hz.shzxlz.cn/gtcgkbspkj.html

[R29] 定义函数
来源：http://hz.zhiwuduotai.top/gtdjjegfko.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ppjwa.cn/gtjomvomyp.html

[R30] 函数返回状态码
来源：http://hz.daxiang520.top/gteyschbxo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgfzy.top/gtdimmfojh.html

[R31] 局部变量
来源：http://hz.xuanzx.com/gtepyhcveu.html

f() { local x=1; echo "$x"; }
来源：http://hz.fzhhl.top/gtolussktk.html

[R32] 参数个数校验
来源：http://hz.pycfn.com/gtojqdwzfp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtudlojnvn.html

[R33] 捕获错误并提示行号
来源：http://hz.cqqwz.cn/gtesclpblw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.havefunace.top/gtuqyuhapm.html

[R34] 退出时清理
来源：http://hz.xingfuxueyuan.xyz/gtqtfncjwk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtmuqjemsd.html

[R35] 后台执行并等待
来源：http://hz.jiagoushi.top/gtadxclugk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tanke756.top/gtsjznyrbc.html

[R36] 并发执行多个任务
来源：http://hz.daria6918.cn/gtzyzgjnto.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shzxlz.cn/gtlmjbauly.html

[R37] 把输出赋给变量
来源：http://hz.ivvv.top/gturgkfuzp.html

files=$(ls -1)
来源：http://hz.yuanzhike.top/gtaohanjea.html

[R38] 管道串联
来源：http://hz.pycfn.com/gttemyqgoj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hysaishi.cn/gtwiqzeuhq.html

[R39] 重定向标准输出与错误
来源：http://hz.gogol.net.cn/gtxtthohdy.html

cmd > out.log 2>&1
来源：http://hz.jqgfzy.top/gtjymtgtoi.html

[R40] 追加写日志
来源：http://hz.fzhhl.top/gtpjqzitek.html

echo "log" >> out.log
来源：http://hz.nanxuanxn.top/gtxwtoltlk.html

[R41] 丢弃输出
来源：http://hz.pycfn.com/gtyuwurhhn.html

cmd >/dev/null 2>&1
来源：http://hz.guowangkeji.top/gtorwtgnxg.html

[R42] 输入重定向
来源：http://hz.cashguo.top/gtxjwoixvg.html

wc -l < a.txt
来源：http://hz.0kj1m.cn/gtzqmvxyam.html

[R43] 按名字查找文件
来源：http://hz.zhengqikj.top/gtqddpcbfx.html

find . -name "*.log" -type f
来源：http://hz.zdqjudy.top/gtwztcmctm.html

[R44] 按修改时间查找
来源：http://hz.yongpay.top/gtulsvfdhj.html

find . -mtime -7 -type f
来源：http://hz.yuxming.cn/gtaqzztodi.html

[R45] 批量删除
来源：http://hz.sysykeji.top/gtbtectmqk.html

find . -name "*.tmp" -delete
来源：http://hz.jinqigfzy.top/gtykufvkrw.html

[R46] 递归替换文件内容
来源：http://hz.wangshuangyany.cn/gtfjobekli.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gttagrahkg.html

[R47] sed 单行替换
来源：http://hz.jlsjyb.cn/gtmhwbxnix.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhoulong.xyz/gtfeapcizk.html

[R48] awk 取指定列
来源：http://hz.ywan-chungtsiang.top/gthhkiwbir.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtgfyujbjc.html

[R49] awk 带条件
来源：http://hz.9152youxi.cn/gtxqwdegtq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.kuanghao11.cn/gtkvsjmvva.html

[R50] awk 求和
来源：http://hz.mhx1999.top/gtzkuaraqt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xuanzx.com/gtovtwlryt.html

[R51] 排序去重取前几
来源：http://hz.wangshuangyany.cn/gtlxophavb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tianlin.xyz/gtojrlvnot.html

[R52] 统计行数
来源：http://hz.sweek.top/gtnncqtomn.html

wc -l a.txt
来源：http://hz.haohaochexian.top/gtxozcsync.html

[R53] 查看文件头与实时尾
来源：http://hz.zdqjudy.top/gtbegppxnw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sufxvd.cn/gtrpdgokoq.html

[R54] 比较两个文件
来源：http://hz.shuidangran.top/gtilnmkxky.html

diff a.txt b.txt
来源：http://hz.gaohongyu789.top/gtefabvpyc.html

[R55] 压缩与解压
来源：http://hz.nanxuanxn.top/gtfyfftcjk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxinkj.top/gtzmlbutet.html

[R56] 远程拷贝
来源：http://hz.jinghuilouyu.cn/gtjadfcbxq.html

scp file user@host:/path/
来源：http://hz.zhixingplan.top/gtzmvozcon.html

[R57] 远程执行命令
来源：http://hz.shuidangran.top/gtvzeeqxey.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtqfvxzfii.html

[R58] 下载文件
来源：http://hz.guannengcc.top/gtariezlar.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenjidiqi.icu/gtgglsxobw.html

[R59] 发 POST JSON
来源：http://hz.xziqi.cn/gtxasvvzpw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gaohongyu789.top/gtzgnderkr.html

[R60] 只看 HTTP 状态码
来源：http://hz.hongshengwenyu.top/gtrtmtkzsu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yanxiufei.cn/gtowqegahs.html

[R61] 磁盘占用
来源：http://hz.sxryk.cn/gtazahnjvv.html

df -h;  du -sh *
来源：http://hz.bjfxy.top/gtdxgchwka.html

[R62] 找最占空间的文件
来源：http://hz.yj202588.top/gtyjlopfjl.html

du -ah . | sort -rh | head -10
来源：http://hz.chenlongwang.top/gtlrxzjjjf.html

[R63] 内存与进程
来源：http://hz.xingfuxueyuan.xyz/gtfylideqn.html

free -h;  ps aux | grep nginx
来源：http://hz.0kj1m.cn/gtyvzgmahx.html

[R64] 结束进程
来源：http://hz.sxryk.cn/gtcqzvelmg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnxiangtu.top/gtqetxlysr.html

[R65] 查看端口占用
来源：http://hz.nanxinkj.top/gtpsynyxui.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenjidiqi.icu/gtzamgzpxn.html

[R66] 定时任务
来源：http://hz.tanke756.top/gtcsnqztll.html

crontab -e;  crontab -l
来源：http://hz.dashuyun.cn/gtkcnoxakl.html

[R67] 生成随机十六进制串
来源：http://hz.ydjk.org.cn/gtigzflgfr.html

openssl rand -hex 16
来源：http://hz.shanyushiyangtech.top/gtqvbbdmmu.html

[R68] 计算文件校验值
来源：http://hz.ydzc1.top/gthqbcwmvd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtsdsjfbqx.html

[R69] 生成随机密码
来源：http://hz.iojbl.cn/gtjditczsy.html

head -c 16 /dev/urandom | base64
来源：http://hz.gaohongyu789.top/gtykchzfqo.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtpzsjpdeo.html

date +%s;  date -d @1700000000
来源：http://hz.yanxiufei.cn/gtpttbucqq.html

[R71] 日期格式化
来源：http://hz.hongshengwenyu.top/gtkubmprtm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gogol.net.cn/gteqwnehrz.html

[R72] 等待端口就绪
来源：http://hz.c1oappe.top/gtynvrzukf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jiagoushi.top/gtnpuccyhl.html

[R73] 分割大日志
来源：http://hz.ehwqpu.com/gtthxxnncj.html

split -l 1000 big.log part_
来源：http://hz.yangfankeji.com/gtisdtjbqu.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gtpwywjaxp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hammf.cn/gtmtitnitf.html

[R75] 导出环境变量
来源：http://hz.zycfv.cn/gtisvibpik.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shuidangran.top/gttnpvswrn.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtominwral.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenzaomai.com/gtgkxqxxxk.html

[R77] 读取用户输入
来源：http://hz.aizwys.cn/gtonhpwimq.html

read -rp "请输入: " ans
来源：http://hz.zhaomingkeji.xyz/gtkclmfnhc.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gtkmjpdost.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yueranfly.top/gtmytwyndn.html

[R79] 解析命令行选项
来源：http://hz.ppjwa.cn/gtljvcidds.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cheryme.top/gtbatklpuq.html

[R80] 查看脚本执行耗时
来源：http://hz.shuidangran.top/gtwnhkoxri.html

time ./run.sh
来源：http://hz.c1oappe.top/gtrpdkrtfb.html

================================================================================
来源：http://hz.iojbl.cn/gtaknikiok.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gtgeshcxdx.html

================================================================================
来源：http://hz.xinyue.icu/gtxtctvabd.html

[S01] C：Hello World
来源：http://hz.shanyushiyangkeji.top/gtoafyizqi.html

#include <stdio.h>
来源：http://hz.daxiang520.top/gtokwfqrce.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zycfv.cn/gtvavkqnud.html

[S02] C：变量与格式化输出
来源：http://hz.yangfankeji.com/gtxbnrcpmg.html

int a = 10; printf("%d\n", a);
来源：http://hz.dashuyun.cn/gtylgzhddk.html

[S03] C：读入整数
来源：http://hz.yj202588.top/gtsyfwlwdm.html

int x; scanf("%d", &x);
来源：http://hz.ehwqpu.com/gtiyculjlh.html

[S04] C：字符串复制
来源：http://hz.nanxinkj.top/gtiltwvnwa.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zdqjudy.top/gtwmkdiuzg.html

[S05] C：字符串长度
来源：http://hz.jinqigfzy.top/gtctnwazqk.html

strlen(s)
来源：http://hz.vqdsnc.cn/gtefzgzftx.html

[S06] C：字符串比较
来源：http://hz.zdqjudy.top/gtdlhrujku.html

strcmp(a, b) == 0
来源：http://hz.gogol.net.cn/gtuyyetrdd.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangtech.top/gthswmfmwi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guowangkeji.top/gtptnysjvl.html

[S08] C：动态内存分配与释放
来源：http://hz.dianchejie.cn/gtzeblnfcu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.9152youxi.cn/gtqwnvbbrw.html

[S09] C：结构体定义与初始化
来源：http://hz.vqdsnc.cn/gtyflqtpou.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xziqi.cn/gtqkxcezud.html

[S10] C：指针与解引用
来源：http://hz.xziqi.cn/gthtlgtiio.html

int *p = &a;  *p = 5;
来源：http://hz.yvedp.cn/gtjetqowoo.html

[S11] C：逐行读文件
来源：http://hz.0kj1m.cn/gtzqhphnay.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhiwuduotai.top/gtrrbrnfls.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aibaodan.cn/gtgnzrrfom.html

fclose(f);
来源：http://hz.jinqigfzy.top/gtdaenuosc.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gtrqtpyxvf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xinyue.icu/gtsxulhgry.html

[S13] C：宏定义
来源：http://hz.xuetiantiany.cn/gtpryivkyk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guowangkeji.top/gtgrsozcvl.html

[S14] C：枚举
来源：http://hz.shanyushiyangtech.top/gtlvhmavcb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.haohaochexian.top/gtsabvrtze.html

[S15] C：类型转换
来源：http://hz.pengpengdd.cyou/gtmxkwyvyx.html

(double) a / b
来源：http://hz.yvedp.cn/gtdohztewq.html

[S16] C：位操作置位
来源：http://hz.yueranfly.top/gtybejrhlt.html

x |= (1 << 3);
来源：http://hz.ehwqpu.com/gtuubjyyql.html

[S17] C：安全拼接字符串
来源：http://hz.hongshengwenyu.top/gtjedmeimn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.redwolf501.top/gtzqonskse.html

[S18] C：命令行参数
来源：http://hz.fengsongda.top/gtapvuragi.html

int main(int argc, char **argv)
来源：http://hz.zycfv.cn/gtmbarjtcw.html

[S19] C：快速排序
来源：http://hz.cdnleiting.top/gtotrxomvu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtjbgfaeoh.html

[S20] C：二分查找
来源：http://hz.yj20258888.top/gthusofvak.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnqzz.top/gtzbhiysly.html

[S21] C：字符类别判断
来源：http://hz.dianchejie.cn/gtxgmechzx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.kuanghao11.cn/gtaldjnuxy.html

[S22] C：字符串转数字
来源：http://hz.hammf.cn/gtlhaawmvx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xingfuxueyuan.xyz/gtrrxugnwy.html

[S23] C：随机数
来源：http://hz.316326.xyz/gtgsizvgsn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtnynqmdrs.html

[S24] C：获取本地时间
来源：http://hz.chenlongwang.top/gtzldsfmdp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.mhx1999.top/gtahpobwum.html

[S25] C：内存拷贝
来源：http://hz.0kj1m.cn/gtndtdzffl.html

memcpy(dst, src, n);
来源：http://hz.xinyue.icu/gtblqnkvxx.html

[S26] C：内存清零
来源：http://hz.daxiang520.top/gtdhwqupte.html

memset(a, 0, sizeof a);
来源：http://hz.yonumen.top/gtlkynrikx.html

[S27] C：定义常量
来源：http://hz.hnqzz.top/gtscaksjxm.html

const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtyzvvmbsb.html

[S28] C：静态变量
来源：http://hz.hnqzz.top/gtjjlbnpej.html

static int counter = 0;
来源：http://hz.xziqi.cn/gtdjclmmlw.html

[S29] C：变参函数
来源：http://hz.zhoulong.xyz/gtwsvguzih.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.9152youxi.cn/gtbelkoyvb.html

[S30] C：头文件保护
来源：http://hz.jiagoushi.top/gtcfpxorip.html

#ifndef X_H
来源：http://hz.jqgufenzy.top/gtrihrahfz.html

#define X_H
来源：http://hz.daxiang520.top/gtszcaropr.html

#endif
来源：http://hz.zhoulong.xyz/gtodlziqhl.html

[S31] C++：Hello World
来源：http://hz.tanke756.top/gtctznqmwb.html

#include <iostream>
来源：http://hz.sxryk.cn/gtnahbbdpe.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nanxinkj.top/gtlzeayqub.html

[S32] C++：字符串
来源：http://hz.gotoacloud.top/gtussdpuyx.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gtlcrciato.html

[S33] C++：vector 增删
来源：http://hz.jinghuilouyu.cn/gtsazhscny.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.feifeiyinyue.top/gtrowgxezj.html

[S34] C++：遍历 vector
来源：http://hz.yuanzhike.top/gtxzcqxfps.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daxiang520.top/gtkdowubrt.html

[S35] C++：map
来源：http://hz.yangfankeji.com/gtssbyjanr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gtqjitafbx.html

[S36] C++：unordered_map
来源：http://hz.yuxming.cn/gtrkipdwcp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtofvrwemk.html

[S37] C++：set
来源：http://hz.yuanzhike.top/gtedaozcgq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gthnczvifo.html

[S38] C++：排序
来源：http://hz.jinqigufen.top/gtqthkdlyi.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgfzy.top/gtofxqugog.html

[S39] C++：自定义比较器排序
来源：http://hz.ywan-chungtsiang.top/gtyuxasnzb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenjidiqi.icu/gtgtwrgfbz.html

[S40] C++：查找元素
来源：http://hz.yanxiufei.cn/gtmkszmgzh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gotoacloud.top/gtjxavnelh.html

[S41] C++：类与构造函数
来源：http://hz.ywan-chungtsiang.top/gttvmxxryc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sufxvd.cn/gtivtraxuo.html

[S42] C++：继承与虚函数
来源：http://hz.fengsongda.top/gtvlepnjjs.html

class B : public Base { public: void f() override {} };
来源：http://hz.cashguo.top/gtabnlnssp.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gtwzazheag.html

auto p = std::make_unique<int>(5);
来源：http://hz.jianghu66.top/gttfutijas.html

[S44] C++：引用传参
来源：http://hz.smart0.xyz/gtowmxzbqd.html

void inc(int &x) { ++x; }
来源：http://hz.yangfankeji.com/gtrujwiway.html

[S45] C++：lambda
来源：http://hz.cqqwz.cn/gtdiybpebm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ppjwa.cn/gtqppujpyu.html

[S46] C++：函数模板
来源：http://hz.ydjk.org.cn/gttatvoyqz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgfzy.top/gtnhhoyohl.html

[S47] C++：结构化绑定遍历
来源：http://hz.gaohongyu789.top/gtkymouzwh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.pycfn.com/gtygjokyzu.html

[S48] C++：逐行读文件
来源：http://hz.chenlongwang.top/gtysehyxiv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.guannengcc.top/gtlruqmsss.html

while (std::getline(in, line)) { }
来源：http://hz.shanyushiyangkeji.top/gtxbuekhyp.html

[S49] C++：写文件
来源：http://hz.316326.xyz/gtnkhrcyzv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shangyingyoupin.top/gtlhsvhelo.html

[S50] C++：格式化数字
来源：http://hz.ybcxt.top/gteskwhsqa.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenjidiqi.icu/gtrkgpbdig.html

[S51] C++：显式类型转换
来源：http://hz.cqqwz.cn/gtasavaros.html

static_cast<double>(a) / b
来源：http://hz.fzhhl.top/gtoigzauty.html

[S52] C++：const 与 noexcept
来源：http://hz.316326.xyz/gtufbmkgbx.html

int size() const noexcept { return n_; }
来源：http://hz.hnxiangtu.top/gttewtqwvh.html

[S53] C++：移动语义
来源：http://hz.dashuyun.cn/gtjifhjtmo.html

std::vector<int> w = std::move(v);
来源：http://hz.tianlin.xyz/gtsansnctw.html

[S54] C++：异常处理
来源：http://hz.hammf.cn/gtxuxupwya.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.aibaodan.cn/gtrihczthu.html

[S55] C++：结构化绑定
来源：http://hz.xinyue.icu/gtnaphuamg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.sufxvd.cn/gtqiiddmtg.html

[S56] C++：optional
来源：http://hz.fzhhl.top/gtcjkggfkd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jianghu66.top/gtnvyajuga.html

[S57] C++：编译期常量
来源：http://hz.tianlin.xyz/gtugjehpaj.html

constexpr int N = 10;
来源：http://hz.fengsongda.top/gtutlqbxbb.html

[S58] C++：命名空间
来源：http://hz.snrcjt.cn/gtgcujlbat.html

namespace ns { int f() { return 1; } }
来源：http://hz.tian-w.cn/gtefydlwci.html

[S59] C++：静态断言
来源：http://hz.meibo888.top/gttntwzptu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgfzy.top/gtvtogtaxe.html

[S60] C++：遍历并删除元素
来源：http://hz.jianghu66.top/gtqvotcfsd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj202588.top/gtnpdoyyin.html

================================================================================
来源：http://hz.pycfn.com/gtyxarrhqh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangtech.top/gtgdxixdje.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthhwyqvro.html

[T01] Kotlin：Hello World
来源：http://hz.gzhubu.top/gtlteroeob.html

println("Hello")
来源：http://hz.tanke756.top/gtwwziidia.html

[T02] Kotlin：变量
来源：http://hz.yanxiufei.cn/gtfkqjvmfj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.c1oappe.top/gtjmyhgpze.html

[T03] Kotlin：字符串模板
来源：http://hz.xinyue.icu/gtiojtkycx.html

"值: $b"
来源：http://hz.chenzaomai.com/gtbqyhygoy.html

[T04] Kotlin：空安全
来源：http://hz.sxryk.cn/gthdvavozw.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtimzrywau.html

[T05] Kotlin：when 表达式
来源：http://hz.ybcxt.top/gtmwyvjncs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydzc1.top/gtbehakkhi.html

[T06] Kotlin：集合映射
来源：http://hz.sufxvd.cn/gtokfpmkog.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yuanzhike.top/gtrawblwfb.html

[T07] Kotlin：集合过滤
来源：http://hz.zycfv.cn/gtxyewwsfr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhaomingkeji.xyz/gtqotfsanm.html

[T08] Kotlin：数据类
来源：http://hz.tanke756.top/gttmopwqea.html

data class User(val name: String, val age: Int)
来源：http://hz.aibaodan.cn/gtuqvupyke.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangkeji.top/gtuwgyvhil.html

fun String.exclaim() = this + "!"
来源：http://hz.smart0.xyz/gtvvuifpwl.html

[T10] Kotlin：默认参数
来源：http://hz.yj20258.top/gtlwcsknao.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.haohaochexian.top/gtjkweiuxl.html

[T11] Kotlin：协程
来源：http://hz.chenlongwang.top/gtvbccrjbf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydzc1.top/gtrnlirwsc.html

[T12] Kotlin：解构声明
来源：http://hz.nanxinkj.top/gtbsoxayct.html

val (a, b) = Pair(1, 2)
来源：http://hz.c1oappe.top/gtyblhlaij.html

[T13] Kotlin：只读 Map
来源：http://hz.kuanghao11.cn/gtpojzuhnu.html

val m = mapOf("a" to 1)
来源：http://hz.feifeiyinyue.top/gttloncfsc.html

[T14] Kotlin：循环
来源：http://hz.jinqigufen.top/gtmvtqtjee.html

for (i in 1..10) println(i)
来源：http://hz.shangyingyoupin.top/gtbrgcvktz.html

[T15] Kotlin：接口
来源：http://hz.guowangkeji.top/gtlnnrmbfb.html

interface Shape { fun area(): Double }
来源：http://hz.tanke756.top/gtqmaxfxmb.html

[T16] Swift：Hello World
来源：http://hz.xylfe.cn/gtiypzpdsp.html

print("Hello")
来源：http://hz.nwbrower.top/gtuqjummnz.html

[T17] Swift：变量与常量
来源：http://hz.yangfankeji.com/gtyeuwtziy.html

var a = 1;  let b = 2
来源：http://hz.ppjwa.cn/gtobwailzm.html

[T18] Swift：字符串插值
来源：http://hz.yonumen.top/gtehmnwnge.html

"值: \(b)"
来源：http://hz.hongshengwenyu.top/gtxwppyixu.html


<!-- 参考信息 -->