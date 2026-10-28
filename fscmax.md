代发 wailian999

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtrupfgtxd.html

SELECT TRIM(name) FROM users;
来源：http://hz.zhijiandao.cn/gtcouqmwlp.html

[Q85] 数值取整
来源：http://hz.hnxiangtu.top/gtgefhlwko.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ydjk.org.cn/gtnfodsewp.html

[Q86] 读取 JSON 字段
来源：http://hz.xziqi.cn/gtrkgffsyy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zycfv.cn/gtwooexzln.html

[Q87] JSON 字段做条件
来源：http://hz.hongshengwenyu.top/gttwxtoihh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zycfv.cn/gtjcdhjcrk.html

[Q88] 行转列（条件聚合）
来源：http://hz.52xcode.cn/gtfajmfufz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yuxming.cn/gtadlywzli.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhijiandao.cn/gtrluijaak.html

[Q89] 判断表是否存在
来源：http://hz.chenlongwang.top/gtqihvjhtm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nanxinkj.top/gtlliyooaz.html

[Q90] 生成序号列
来源：http://hz.vqdsnc.cn/gttoousuvb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gtwfvcdfub.html

================================================================================
来源：http://hz.daxiang520.top/gthrtwaosd.html

R. Bash 专题
来源：http://hz.hywenlv.cn/gtktquwlvk.html

================================================================================
来源：http://hz.aizwys.cn/gteimpvvmi.html

[R01] shebang 与严格模式
来源：http://hz.andypj.xyz/gtbvrqlywc.html

#!/usr/bin/env bash
来源：http://hz.cucudq.cn/gtdfoptqep.html

set -euo pipefail
来源：http://hz.sweek.top/gtetfrxrjd.html

[R02] 变量赋值与使用
来源：http://hz.ehwqpu.com/gtybcmhlzj.html

name="Tom"; echo "$name"
来源：http://hz.ywan-chungtsiang.top/gtlaucyzyj.html

[R03] 只读变量
来源：http://hz.nanxuanxn.top/gtggqvbhvj.html

readonly PI=3.14
来源：http://hz.zdqjudy.top/gterzkskci.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gtmdhkzeir.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nanxuanxn.top/gtilrxyczi.html

[R05] 参数默认值
来源：http://hz.hammf.cn/gtnhnesvxk.html

name="${1:-default}"
来源：http://hz.birdmap.top/gtididlqtp.html

[R06] 判断命令是否存在
来源：http://hz.birdmap.top/gtuonlybvh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cdnleiting.top/gtychbcnyp.html

[R07] if 判断文件
来源：http://hz.fzhhl.top/gtpvxltwpk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sysykeji.top/gtkhtkegai.html

[R08] 数值比较
来源：http://hz.chenzaomai.com/gtgzblbcdp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zycfv.cn/gtczrmnucl.html

[R09] 字符串比较
来源：http://hz.wangdashe.top/gtefxckzwg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tian-w.cn/gtuultdnxl.html

[R10] 正则匹配
来源：http://hz.0kj1m.cn/gtrlllxiop.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zycfv.cn/gtoyjuvxck.html

[R11] case 多分支
来源：http://hz.jianghu66.top/gtwryzojcp.html

case "$1" in
来源：http://hz.yangfankeji.com/gtnbwagtjr.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtievbxbtd.html

stop)  echo "停止" ;;
来源：http://hz.aibaodan.cn/gtbxsyozse.html

*)     echo "未知命令" ;;
来源：http://hz.cheryme.top/gttaklovfq.html

esac
来源：http://hz.nanxuanxn.top/gtflvvsnsz.html

[R12] for 遍历文件
来源：http://hz.tian-w.cn/gtcomajype.html

for f in *.txt; do echo "$f"; done
来源：http://hz.guowangkeji.top/gttnzfacfc.html

[R13] for 计数循环
来源：http://hz.shanyushiyangtech.top/gtzapeszfx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tanke756.top/gtujazwvjt.html

[R14] C 风格 for
来源：http://hz.xingfuxueyuan.xyz/gtkhvudfwm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cdnleiting.top/gtzsygxflr.html

[R15] while 逐行读文件
来源：http://hz.dashuyun.cn/gtfhhbppwy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daxiang520.top/gtmjcsxzue.html

[R16] until 等待条件
来源：http://hz.cdnleiting.top/gtfzkexcby.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zycfv.cn/gtvzsytdfu.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtomdpnirx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xylfe.cn/gtzfnnfmvb.html

[R18] 遍历数组
来源：http://hz.ppjwa.cn/gtlnkgpuse.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.0kj1m.cn/gtinndlkze.html

[R19] 数组长度
来源：http://hz.chenzaomai.com/gtgpxejflf.html

echo "${#arr[@]}"
来源：http://hz.jinqigfzy.top/gtuheoikwv.html

[R20] 关联数组（字典）
来源：http://hz.andypj.xyz/gtauyxzipz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gogol.net.cn/gtspjqkbbh.html

[R21] 字符串长度
来源：http://hz.xuanzx.com/gtccneexlq.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gtzxigcuyo.html

[R22] 截取子串
来源：http://hz.guowangkeji.top/gtijvfoivl.html

echo "${s:0:5}"
来源：http://hz.wangshuangyany.cn/gtanxoydlq.html

[R23] 字符串替换
来源：http://hz.0kj1m.cn/gteboqzjtv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhixingplan.top/gthqeswkxf.html

[R24] 大小写转换
来源：http://hz.jinqigfzy.top/gtmvxncbbh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tian-w.cn/gtvigstjkk.html

[R25] 去后缀 / 去前缀
来源：http://hz.havefunace.top/gtmunfljze.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shuidangran.top/gtvxvxvaxa.html

[R26] 命令替换
来源：http://hz.ydzc1.top/gtityawviz.html

now=$(date +%F); echo "$now"
来源：http://hz.ydjk.org.cn/gtabfrjiti.html

[R27] 算术展开
来源：http://hz.cucudq.cn/gtnlncjegf.html

echo $((1 + 2 * 3))
来源：http://hz.yanxiufei.cn/gtmoncsysm.html

[R28] 浮点运算
来源：http://hz.hongshengwenyu.top/gtjcgkwhrs.html

echo "scale=2; 10/3" | bc
来源：http://hz.cashguo.top/gttplmuhla.html

[R29] 定义函数
来源：http://hz.hongshengwenyu.top/gtzfrlkdxe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dashuyun.cn/gthghuzfvx.html

[R30] 函数返回状态码
来源：http://hz.guowangkeji.top/gtzqnylnxq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.meibo888.top/gttmieaael.html

[R31] 局部变量
来源：http://hz.jlsjyb.cn/gtldwewugp.html

f() { local x=1; echo "$x"; }
来源：http://hz.zdqjudy.top/gttmwwlolq.html

[R32] 参数个数校验
来源：http://hz.nanxuanxn.top/gtxmuqyhbh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.pycfn.com/gtwjiqeicl.html

[R33] 捕获错误并提示行号
来源：http://hz.haohaochexian.top/gtbgadcndy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cqqwz.cn/gtefzpnaiy.html

[R34] 退出时清理
来源：http://hz.birdmap.top/gtfakmevmo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gtsjbllsvh.html

[R35] 后台执行并等待
来源：http://hz.smart0.xyz/gtzaombvvi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cdnleiting.top/gtlzfxcekb.html

[R36] 并发执行多个任务
来源：http://hz.pengpengdd.cyou/gtnnspywob.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pengpengdd.cyou/gtmcqtzjsp.html

[R37] 把输出赋给变量
来源：http://hz.yuanzhike.top/gtmtzklffh.html

files=$(ls -1)
来源：http://hz.yanxiufei.cn/gtvjvermeb.html

[R38] 管道串联
来源：http://hz.feifeiyinyue.top/gtnsjlbila.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hywenlv.cn/gtymjrdbhk.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gtttlymkyx.html

cmd > out.log 2>&1
来源：http://hz.cashguo.top/gtdtmkgeps.html

[R40] 追加写日志
来源：http://hz.yj202588.top/gtemvrmkll.html

echo "log" >> out.log
来源：http://hz.tian-w.cn/gtwtmgnemd.html

[R41] 丢弃输出
来源：http://hz.fengsongda.top/gtoamvlugh.html

cmd >/dev/null 2>&1
来源：http://hz.kuanghao11.cn/gtgbhmnalh.html

[R42] 输入重定向
来源：http://hz.xuetiantiany.cn/gtiqyqyrzi.html

wc -l < a.txt
来源：http://hz.jinqigfzy.top/gtqqloocrd.html

[R43] 按名字查找文件
来源：http://hz.bjfxy.top/gttbktbior.html

find . -name "*.log" -type f
来源：http://hz.jinqigfzy.top/gtfdragaam.html

[R44] 按修改时间查找
来源：http://hz.jinqigfzy.top/gtnwqwexbu.html

find . -mtime -7 -type f
来源：http://hz.ydzc1.top/gtdpyandjh.html

[R45] 批量删除
来源：http://hz.hysaishi.cn/gtnjnqpjna.html

find . -name "*.tmp" -delete
来源：http://hz.dashuyun.cn/gtmoepsqmn.html

[R46] 递归替换文件内容
来源：http://hz.quarkkingdee.top/gtnrappdum.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jiagoushi.top/gtlkhqizsm.html

[R47] sed 单行替换
来源：http://hz.fzhhl.top/gtsxjhamff.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yvedp.cn/gtwejpcwjf.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gtjsxdndaz.html

awk '{print $1, $3}' a.txt
来源：http://hz.xuetiantiany.cn/gtlprcgeyz.html

[R49] awk 带条件
来源：http://hz.gzhubu.top/gtutbtvjll.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tianlin.xyz/gtjtralmxf.html

[R50] awk 求和
来源：http://hz.hammf.cn/gtyhyakqol.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guowangkeji.top/gtzcxddjva.html

[R51] 排序去重取前几
来源：http://hz.shangyingyoupin.top/gtendctwnd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinyuanbaomall.cn/gtlnhhvwwd.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtqnxjfuor.html

wc -l a.txt
来源：http://hz.snrcjt.cn/gtqvcvzxen.html

[R53] 查看文件头与实时尾
来源：http://hz.havefunace.top/gtolfgdcwu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtyxzohwnz.html

[R54] 比较两个文件
来源：http://hz.xuanzx.com/gtvfrxcnbc.html

diff a.txt b.txt
来源：http://hz.daxiang520.top/gtctaiirht.html

[R55] 压缩与解压
来源：http://hz.zycfv.cn/gtnvsfordr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.bjfxy.top/gtkrwegyaw.html

[R56] 远程拷贝
来源：http://hz.svipenyu.cn/gtalhfhhqc.html

scp file user@host:/path/
来源：http://hz.pengpengdd.cyou/gtwkqvatkp.html

[R57] 远程执行命令
来源：http://hz.nwbrower.top/gtdyqslams.html

ssh user@host 'uptime'
来源：http://hz.cucudq.cn/gtiojemvbs.html

[R58] 下载文件
来源：http://hz.yj20258.top/gthodrxrnu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yanxiufei.cn/gtorokqdtn.html

[R59] 发 POST JSON
来源：http://hz.yj202588.top/gtamauosfw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtqbxcfrjj.html

[R60] 只看 HTTP 状态码
来源：http://hz.birdmap.top/gtgpiqbizw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pycfn.com/gtwewaftjr.html

[R61] 磁盘占用
来源：http://hz.hnxiangtu.top/gtesulhuvn.html

df -h;  du -sh *
来源：http://hz.andypj.xyz/gthvdblkyo.html

[R62] 找最占空间的文件
来源：http://hz.ehwqpu.com/gtkxtwtcsl.html

du -ah . | sort -rh | head -10
来源：http://hz.snrcjt.cn/gtakowlbtd.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gteakjivjt.html

free -h;  ps aux | grep nginx
来源：http://hz.aizwys.cn/gtphvghlnr.html

[R64] 结束进程
来源：http://hz.zdqjudy.top/gtuqvdtihv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.birdmap.top/gtidedbbzk.html

[R65] 查看端口占用
来源：http://hz.hysaishi.cn/gtdrraqley.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jlsjyb.cn/gtemojnqvu.html

[R66] 定时任务
来源：http://hz.dianchejie.cn/gtkarqgzdj.html

crontab -e;  crontab -l
来源：http://hz.zycfv.cn/gtzndmdgni.html

[R67] 生成随机十六进制串
来源：http://hz.quarkkingdee.top/gtngctmbqe.html

openssl rand -hex 16
来源：http://hz.hywenlv.cn/gtcoflrlxa.html

[R68] 计算文件校验值
来源：http://hz.hongshengwenyu.top/gtomzmhmio.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dianchejie.cn/gtijugvabu.html

[R69] 生成随机密码
来源：http://hz.ywan-chungtsiang.top/gtarpyccgp.html

head -c 16 /dev/urandom | base64
来源：http://hz.gzhubu.top/gtoxtqnahp.html

[R70] 时间戳与互转
来源：http://hz.316326.xyz/gtkppzrjfk.html

date +%s;  date -d @1700000000
来源：http://hz.hywenlv.cn/gtggymtryu.html

[R71] 日期格式化
来源：http://hz.iojbl.cn/gtfbvyqjbm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shanyushiyangkeji.top/gtmpgnkjun.html

[R72] 等待端口就绪
来源：http://hz.sxryk.cn/gtcvuhiryc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yanxiufei.cn/gtezzdzrxm.html

[R73] 分割大日志
来源：http://hz.shzxlz.cn/gtnyphmaoh.html

split -l 1000 big.log part_
来源：http://hz.yanxiufei.cn/gtvihvgaht.html

[R74] 批量重命名
来源：http://hz.iojbl.cn/gtkitwjrid.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtsuolzrbp.html

[R75] 导出环境变量
来源：http://hz.havefunace.top/gtuubogogw.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhongyouzk.top/gtwrmbcrmg.html

[R76] 使用临时文件
来源：http://hz.cucudq.cn/gtcbiwuiey.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtbcpzkokb.html

[R77] 读取用户输入
来源：http://hz.jinqigfzy.top/gtbpkzwqlz.html

read -rp "请输入: " ans
来源：http://hz.xinyue.icu/gtdghuaogc.html

[R78] 交互式菜单
来源：http://hz.vqdsnc.cn/gtvpdlclfn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhongyouzk.top/gthjrjesjf.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtotxsibcf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yj202588.top/gtxfaslpwj.html

[R80] 查看脚本执行耗时
来源：http://hz.316326.xyz/gtimpvnjen.html

time ./run.sh
来源：http://hz.sweek.top/gtkszsnycg.html

================================================================================
来源：http://hz.xinyue.icu/gtwoprbngf.html

S. C / C++ 专题
来源：http://hz.yanxiufei.cn/gtiigpmjhv.html

================================================================================
来源：http://hz.jlsjyb.cn/gtsnmfhgrg.html

[S01] C：Hello World
来源：http://hz.fzhhl.top/gtvhtbibhs.html

#include <stdio.h>
来源：http://hz.haohaochexian.top/gtmfroqpzm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xinyue.icu/gtvuplkklv.html

[S02] C：变量与格式化输出
来源：http://hz.hongshengwenyu.top/gtnbltwzuq.html

int a = 10; printf("%d\n", a);
来源：http://hz.cucudq.cn/gtlpppliij.html

[S03] C：读入整数
来源：http://hz.nanxuanxn.top/gtqfsumgtk.html

int x; scanf("%d", &x);
来源：http://hz.ppjwa.cn/gtqjkwkcrl.html

[S04] C：字符串复制
来源：http://hz.sweek.top/gtfddapalc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ehwqpu.com/gtyrzrtpli.html

[S05] C：字符串长度
来源：http://hz.52xcode.cn/gtqrougfzz.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gtidinagms.html

[S06] C：字符串比较
来源：http://hz.smart0.xyz/gtjpzvzsds.html

strcmp(a, b) == 0
来源：http://hz.yuanzhike.top/gtfnmolybf.html

[S07] C：数组遍历求和
来源：http://hz.ydjk.org.cn/gtsuiyrunh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnqzz.top/gtalqbmoki.html

[S08] C：动态内存分配与释放
来源：http://hz.ybcxt.top/gtpfzpyrca.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shzxlz.cn/gtsjowmyqf.html

[S09] C：结构体定义与初始化
来源：http://hz.shuidangran.top/gtfpuklqrd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aibaodan.cn/gtcrfsoukh.html

[S10] C：指针与解引用
来源：http://hz.jqgufenzy.top/gtcxvgnedy.html

int *p = &a;  *p = 5;
来源：http://hz.dianchejie.cn/gtbavyjydd.html

[S11] C：逐行读文件
来源：http://hz.316326.xyz/gttmmmltmt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhaomingkeji.xyz/gtyqshropd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yuxming.cn/gtdyprazag.html

fclose(f);
来源：http://hz.guannengcc.top/gtubbfdjfo.html

[S12] C：写文件
来源：http://hz.andypj.xyz/gtxpvvgeyc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gtcqnbcaeb.html

[S13] C：宏定义
来源：http://hz.mhx1999.top/gtaetathmb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jlsjyb.cn/gttpxmoivq.html

[S14] C：枚举
来源：http://hz.fzhhl.top/gtrzoguwhk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhongyouzk.top/gtsmaimiwg.html

[S15] C：类型转换
来源：http://hz.zhongyouzk.top/gtsnqszpku.html

(double) a / b
来源：http://hz.jinyuanbaomall.cn/gtpchovgel.html

[S16] C：位操作置位
来源：http://hz.tanke756.top/gtuxanijtn.html

x |= (1 << 3);
来源：http://hz.xinyue.icu/gtjxakzack.html

[S17] C：安全拼接字符串
来源：http://hz.pycfn.com/gtzdnlthux.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhengqikj.top/gtfqzsbnbv.html

[S18] C：命令行参数
来源：http://hz.jiagoushi.top/gtqvlijhuk.html

int main(int argc, char **argv)
来源：http://hz.shanyushiyangtech.top/gtdjsagvpx.html

[S19] C：快速排序
来源：http://hz.birdmap.top/gtxgiuxvwq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jinghuilouyu.cn/gtffxelqgo.html

[S20] C：二分查找
来源：http://hz.gzhubu.top/gtxkytvzqs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtxrojjfkb.html

[S21] C：字符类别判断
来源：http://hz.sufxvd.cn/gtxciadtix.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.iojbl.cn/gtkkwoilgd.html

[S22] C：字符串转数字
来源：http://hz.svipenyu.cn/gthrypzvsg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ydjk.org.cn/gthpmorudw.html

[S23] C：随机数
来源：http://hz.yonumen.top/gtlwnclarb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gogol.net.cn/gtryoagpxz.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gthklzlasg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.aizwys.cn/gtgxqqxusa.html

[S25] C：内存拷贝
来源：http://hz.tanke756.top/gtfhbxjwzq.html

memcpy(dst, src, n);
来源：http://hz.sweek.top/gtaaciecjw.html

[S26] C：内存清零
来源：http://hz.yuanzhike.top/gtehsjxqfc.html

memset(a, 0, sizeof a);
来源：http://hz.ydzc1.top/gtrvywinkc.html

[S27] C：定义常量
来源：http://hz.sweek.top/gttjlhjefk.html

const double PI = 3.14159;
来源：http://hz.yj20258.top/gtefuwxygu.html

[S28] C：静态变量
来源：http://hz.shuidangran.top/gtzpwcwyos.html

static int counter = 0;
来源：http://hz.pycfn.com/gtnwsbwmbu.html

[S29] C：变参函数
来源：http://hz.yj20258.top/gtdeemmxaa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sxryk.cn/gtbvodcehw.html

[S30] C：头文件保护
来源：http://hz.xziqi.cn/gtnqyvgkfp.html

#ifndef X_H
来源：http://hz.feifeiyinyue.top/gtlqntqrsa.html

#define X_H
来源：http://hz.quarkkingdee.top/gtibbntglt.html

#endif
来源：http://hz.cqqwz.cn/gtvvvzbsxb.html

[S31] C++：Hello World
来源：http://hz.iojbl.cn/gtlheshpiy.html

#include <iostream>
来源：http://hz.cheryme.top/gtwnkhrkms.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tanke756.top/gtcyuxmlsv.html

[S32] C++：字符串
来源：http://hz.hfpthk.cn/gtcobebwkm.html

std::string s = "hi";  s += "!";
来源：http://hz.zhijiandao.cn/gtfkqirxfw.html

[S33] C++：vector 增删
来源：http://hz.ywan-chungtsiang.top/gtwxozkobi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.316326.xyz/gtwjokrgfa.html

[S34] C++：遍历 vector
来源：http://hz.quarkkingdee.top/gtrcagxmqc.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.0kj1m.cn/gtyotwntxo.html

[S35] C++：map
来源：http://hz.xuanzx.com/gttasxpyxt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgufenzy.top/gtmvspolwv.html

[S36] C++：unordered_map
来源：http://hz.xuanzx.com/gtpthytkai.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yangfankeji.com/gtryrksrul.html

[S37] C++：set
来源：http://hz.zhaomingkeji.xyz/gtjynmvwuy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cashguo.top/gtcbvfmzig.html

[S38] C++：排序
来源：http://hz.jiagoushi.top/gtncnafslj.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtxgmdwtjy.html

[S39] C++：自定义比较器排序
来源：http://hz.fengsongda.top/gtxefdiyrv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.9152youxi.cn/gtbamoxuai.html

[S40] C++：查找元素
来源：http://hz.52xcode.cn/gtsiweibws.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtxmswfrvu.html

[S41] C++：类与构造函数
来源：http://hz.daria6918.cn/gtvjmxtrlm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhongyouzk.top/gtqpiiezuv.html

[S42] C++：继承与虚函数
来源：http://hz.feifeiyinyue.top/gtyrjwkbwi.html

class B : public Base { public: void f() override {} };
来源：http://hz.hongshengwenyu.top/gtiroxjtej.html

[S43] C++：智能指针
来源：http://hz.sufxvd.cn/gtxjbhznir.html

auto p = std::make_unique<int>(5);
来源：http://hz.gogol.net.cn/gtruyvxqcn.html

[S44] C++：引用传参
来源：http://hz.yonumen.top/gtgpmddxmk.html

void inc(int &x) { ++x; }
来源：http://hz.jinqigufen.top/gtjfdwwrsh.html

[S45] C++：lambda
来源：http://hz.pengpengdd.cyou/gtlijzmodb.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.guowangkeji.top/gtzhsfoago.html

[S46] C++：函数模板
来源：http://hz.xuetiantiany.cn/gtchiksytt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pycfn.com/gtpezazark.html

[S47] C++：结构化绑定遍历
来源：http://hz.sufxvd.cn/gtwmsrokrh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.haohaochexian.top/gtqcfgmooq.html

[S48] C++：逐行读文件
来源：http://hz.redwolf501.top/gtydppfvah.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtjekhelwx.html

while (std::getline(in, line)) { }
来源：http://hz.yj20258.top/gtbyghyhkh.html

[S49] C++：写文件
来源：http://hz.fengsongda.top/gtvyqfzkvz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cashguo.top/gtoctdjbhh.html

[S50] C++：格式化数字
来源：http://hz.yangfankeji.com/gtidfmsmiw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxuanxn.top/gtpxigwpyk.html

[S51] C++：显式类型转换
来源：http://hz.feifeiyinyue.top/gtjqyofcaf.html

static_cast<double>(a) / b
来源：http://hz.aibaodan.cn/gtgscyczxw.html

[S52] C++：const 与 noexcept
来源：http://hz.ydzc1.top/gtnsahjlni.html

int size() const noexcept { return n_; }
来源：http://hz.hongshengwenyu.top/gtesdkclhq.html

[S53] C++：移动语义
来源：http://hz.xylfe.cn/gtefoungmk.html

std::vector<int> w = std::move(v);
来源：http://hz.cheryme.top/gtzabmgkod.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtfdcbcist.html


<!-- 参考信息 -->