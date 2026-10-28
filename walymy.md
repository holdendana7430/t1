代发 wailian999

[Q84] 去除首尾空格
来源：http://hz.daxiang520.top/gtuomuwsiy.html

SELECT TRIM(name) FROM users;
来源：http://hz.hammf.cn/gtntmjztda.html

[Q85] 数值取整
来源：http://hz.jqgufenzy.top/gtwuqetzia.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shuidangran.top/gtujfljzio.html

[Q86] 读取 JSON 字段
来源：http://hz.shzxlz.cn/gtxdimfoxq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cqqwz.cn/gtzzzfjdwo.html

[Q87] JSON 字段做条件
来源：http://hz.birdmap.top/gthihdlkbl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.cdnleiting.top/gtgvuxnlsx.html

[Q88] 行转列（条件聚合）
来源：http://hz.quarkkingdee.top/gteqysldpw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj202588.top/gtkanpipfo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenzaomai.com/gtjxgbhfrp.html

[Q89] 判断表是否存在
来源：http://hz.zhijiandao.cn/gtpdoaobga.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhiwuduotai.top/gtesaiuyim.html

[Q90] 生成序号列
来源：http://hz.zhoulong.xyz/gtgelkxrpm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shuidangran.top/gthdlicflf.html

================================================================================
来源：http://hz.cqqwz.cn/gtxbqgwowg.html

R. Bash 专题
来源：http://hz.shzxlz.cn/gtsvrlustd.html

================================================================================
来源：http://hz.shuidangran.top/gtkzvqjuvj.html

[R01] shebang 与严格模式
来源：http://hz.jinqigfzy.top/gttsesuiua.html

#!/usr/bin/env bash
来源：http://hz.nanxuanxn.top/gtxxsakdqc.html

set -euo pipefail
来源：http://hz.pycfn.com/gtlmdhgkzb.html

[R02] 变量赋值与使用
来源：http://hz.ydjk.org.cn/gtiajkfynx.html

name="Tom"; echo "$name"
来源：http://hz.yuxming.cn/gtghwusbdv.html

[R03] 只读变量
来源：http://hz.yangfankeji.com/gtujzjznrb.html

readonly PI=3.14
来源：http://hz.9152youxi.cn/gttpvvxvhz.html

[R04] 位置参数
来源：http://hz.yvedp.cn/gthiztcemf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.aizwys.cn/gtzgpquckw.html

[R05] 参数默认值
来源：http://hz.cucudq.cn/gtbdjwspfa.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtudcbeodw.html

[R06] 判断命令是否存在
来源：http://hz.zhongyouzk.top/gtiiydiskl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtsrjnnust.html

[R07] if 判断文件
来源：http://hz.ppjwa.cn/gtdmgkpxwa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yonumen.top/gtvdzzqeqw.html

[R08] 数值比较
来源：http://hz.feifeiyinyue.top/gtbesbebgv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.dashuyun.cn/gtwkitnndf.html

[R09] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtmkakcrwl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinyuanbaomall.cn/gttyrfegup.html

[R10] 正则匹配
来源：http://hz.pengpengdd.cyou/gtskrfljyv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dashuyun.cn/gtpbtdvszd.html

[R11] case 多分支
来源：http://hz.tianlin.xyz/gtjlmjwbno.html

case "$1" in
来源：http://hz.guannengcc.top/gtbxidjebq.html

start) echo "启动" ;;
来源：http://hz.hongshengwenyu.top/gtvokpzazk.html

stop)  echo "停止" ;;
来源：http://hz.meibo888.top/gtuuezfjeo.html

*)     echo "未知命令" ;;
来源：http://hz.hnxiangtu.top/gtwehqbect.html

esac
来源：http://hz.pycfn.com/gtnkrznwym.html

[R12] for 遍历文件
来源：http://hz.hammf.cn/gtvzqwhmtu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zdqjudy.top/gtdxwhignd.html

[R13] for 计数循环
来源：http://hz.ydjk.org.cn/gtvybndvcd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zycfv.cn/gtvfszbihj.html

[R14] C 风格 for
来源：http://hz.yonumen.top/gtdbetqjot.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.cdnleiting.top/gtiidthbhl.html

[R15] while 逐行读文件
来源：http://hz.gaohongyu789.top/gtltxxmbgj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yvedp.cn/gtqadscapu.html

[R16] until 等待条件
来源：http://hz.hywenlv.cn/gtvkweakna.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.andypj.xyz/gteghtdasi.html

[R17] 数组定义与取值
来源：http://hz.wangdashe.top/gtiaqpfqtr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sweek.top/gtzrzwukkt.html

[R18] 遍历数组
来源：http://hz.cashguo.top/gtqmnkmwhg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zycfv.cn/gtgjmgeafm.html

[R19] 数组长度
来源：http://hz.gotoacloud.top/gtzlpjutza.html

echo "${#arr[@]}"
来源：http://hz.yj20258.top/gtpnpghbpx.html

[R20] 关联数组（字典）
来源：http://hz.jqgufenzy.top/gtxmxhajjm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.haohaochexian.top/gtfsifekzs.html

[R21] 字符串长度
来源：http://hz.feifeiyinyue.top/gttpzopmrs.html

echo "${#s}"
来源：http://hz.vqdsnc.cn/gtceaybyra.html

[R22] 截取子串
来源：http://hz.shzxlz.cn/gtchzztnek.html

echo "${s:0:5}"
来源：http://hz.cdnleiting.top/gtabvkaasb.html

[R23] 字符串替换
来源：http://hz.52xcode.cn/gtsbecogpg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aibaodan.cn/gtysxwwjmq.html

[R24] 大小写转换
来源：http://hz.hysaishi.cn/gtjvfgcoxj.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ybcxt.top/gtnociznix.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangdashe.top/gtyaitmjez.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aizwys.cn/gtpfipqudm.html

[R26] 命令替换
来源：http://hz.ehwqpu.com/gtxkwjpmro.html

now=$(date +%F); echo "$now"
来源：http://hz.zdqjudy.top/gtbsfdtlma.html

[R27] 算术展开
来源：http://hz.jlsjyb.cn/gtnzgzrsws.html

echo $((1 + 2 * 3))
来源：http://hz.sweek.top/gtdayhkkjf.html

[R28] 浮点运算
来源：http://hz.xuetiantiany.cn/gtiikloitt.html

echo "scale=2; 10/3" | bc
来源：http://hz.tian-w.cn/gtmewcyybf.html

[R29] 定义函数
来源：http://hz.dianchejie.cn/gthxqmcpmi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtiihtzsnp.html

[R30] 函数返回状态码
来源：http://hz.tian-w.cn/gthoiyawkt.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.aibaodan.cn/gtojlotzkf.html

[R31] 局部变量
来源：http://hz.fengsongda.top/gtievtyxlr.html

f() { local x=1; echo "$x"; }
来源：http://hz.bjfxy.top/gtujduvsoi.html

[R32] 参数个数校验
来源：http://hz.shuidangran.top/gthqlcufrs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jiagoushi.top/gtwmfmwlyt.html

[R33] 捕获错误并提示行号
来源：http://hz.mhx1999.top/gtdkfenrmb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hfpthk.cn/gtwojcgbdg.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtltghbfzx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtshszubzj.html

[R35] 后台执行并等待
来源：http://hz.zycfv.cn/gtzquqivia.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guannengcc.top/gtmtjyfvzi.html

[R36] 并发执行多个任务
来源：http://hz.chenjidiqi.icu/gtnxxgeoif.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.aizwys.cn/gtmwcpafuj.html

[R37] 把输出赋给变量
来源：http://hz.zhijiandao.cn/gttuibivjk.html

files=$(ls -1)
来源：http://hz.vqdsnc.cn/gtxrzhrlyp.html

[R38] 管道串联
来源：http://hz.daria6918.cn/gtvdfdmkhb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gttxvejmwz.html

[R39] 重定向标准输出与错误
来源：http://hz.ivvv.top/gtcsybhevi.html

cmd > out.log 2>&1
来源：http://hz.wangshuangyany.cn/gtjxtthfyr.html

[R40] 追加写日志
来源：http://hz.yanxiufei.cn/gtdlyqqymd.html

echo "log" >> out.log
来源：http://hz.52xcode.cn/gtupbosgzs.html

[R41] 丢弃输出
来源：http://hz.aizwys.cn/gtyposwbze.html

cmd >/dev/null 2>&1
来源：http://hz.iojbl.cn/gticpvrvxf.html

[R42] 输入重定向
来源：http://hz.gogol.net.cn/gthufslcjj.html

wc -l < a.txt
来源：http://hz.shanyushiyangtech.top/gtisuxtmvq.html

[R43] 按名字查找文件
来源：http://hz.aibaodan.cn/gtpyhnpzpg.html

find . -name "*.log" -type f
来源：http://hz.xylfe.cn/gtrjgizzfg.html

[R44] 按修改时间查找
来源：http://hz.tianlin.xyz/gtupsyfqoq.html

find . -mtime -7 -type f
来源：http://hz.tian-w.cn/gtecyfnkmy.html

[R45] 批量删除
来源：http://hz.wangshuangyany.cn/gtwmdstjxn.html

find . -name "*.tmp" -delete
来源：http://hz.yongpay.top/gtnohucazg.html

[R46] 递归替换文件内容
来源：http://hz.yongpay.top/gtxilxvyhr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cheryme.top/gtfhrrusbc.html

[R47] sed 单行替换
来源：http://hz.hnqzz.top/gtveeypfbq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydzc1.top/gthlxbjjqt.html

[R48] awk 取指定列
来源：http://hz.tanke756.top/gtncpfxknd.html

awk '{print $1, $3}' a.txt
来源：http://hz.andypj.xyz/gtdvnmbsty.html

[R49] awk 带条件
来源：http://hz.jianghu66.top/gtzuedsytw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhijiandao.cn/gtibzhxavy.html

[R50] awk 求和
来源：http://hz.pengpengdd.cyou/gtxzpuokzc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yvedp.cn/gttwuvjvob.html

[R51] 排序去重取前几
来源：http://hz.tian-w.cn/gtiwvfdclv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.redwolf501.top/gtnvhkjkdz.html

[R52] 统计行数
来源：http://hz.ehwqpu.com/gtcmttdoyw.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gtvnenxlmz.html

[R53] 查看文件头与实时尾
来源：http://hz.smart0.xyz/gtqhtjupbo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtvagwsgpl.html

[R54] 比较两个文件
来源：http://hz.jqgufenzy.top/gtcrgivxzs.html

diff a.txt b.txt
来源：http://hz.tanke756.top/gtbgusqbqz.html

[R55] 压缩与解压
来源：http://hz.xziqi.cn/gtymdagcae.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.c1oappe.top/gtnekvcfby.html

[R56] 远程拷贝
来源：http://hz.shanyushiyangkeji.top/gtcqkpgkxy.html

scp file user@host:/path/
来源：http://hz.wangshuangyany.cn/gtwphtpcdg.html

[R57] 远程执行命令
来源：http://hz.zycfv.cn/gtftszuowg.html

ssh user@host 'uptime'
来源：http://hz.nanxinkj.top/gtxoybfpdq.html

[R58] 下载文件
来源：http://hz.zycfv.cn/gtjigsgjma.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yuxming.cn/gtrcsdmmtb.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtalzmrywa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.sweek.top/gthkyatqoh.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtkqstfboi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yongpay.top/gtvwrsnwwk.html

[R61] 磁盘占用
来源：http://hz.xylfe.cn/gtjcbjllnk.html

df -h;  du -sh *
来源：http://hz.tian-w.cn/gtciicrunw.html

[R62] 找最占空间的文件
来源：http://hz.quarkkingdee.top/gtdhfwdvvv.html

du -ah . | sort -rh | head -10
来源：http://hz.cdnleiting.top/gtimxfxkxm.html

[R63] 内存与进程
来源：http://hz.yvedp.cn/gtafgschuv.html

free -h;  ps aux | grep nginx
来源：http://hz.guowangkeji.top/gtprelpizm.html

[R64] 结束进程
来源：http://hz.svipenyu.cn/gtuxnkotdn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.c1oappe.top/gtclmvndjs.html

[R65] 查看端口占用
来源：http://hz.0kj1m.cn/gtqeybzejy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangkeji.top/gtmosfsqcn.html

[R66] 定时任务
来源：http://hz.ydjk.org.cn/gtbyvitxft.html

crontab -e;  crontab -l
来源：http://hz.zhongyouzk.top/gtlrzbllrs.html

[R67] 生成随机十六进制串
来源：http://hz.yanxiufei.cn/gthtgvwvqf.html

openssl rand -hex 16
来源：http://hz.yanxiufei.cn/gtpeijzfbd.html

[R68] 计算文件校验值
来源：http://hz.chenlongwang.top/gtchmtxpnw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cheryme.top/gtqczifseq.html

[R69] 生成随机密码
来源：http://hz.zhongyouzk.top/gtunmflhzo.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj202588.top/gtrcdvaegr.html

[R70] 时间戳与互转
来源：http://hz.jinyuanbaomall.cn/gtehoamhia.html

date +%s;  date -d @1700000000
来源：http://hz.hongshengwenyu.top/gtfmguiajf.html

[R71] 日期格式化
来源：http://hz.sxryk.cn/gtcnimzkeb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuxming.cn/gtiuspkcuk.html

[R72] 等待端口就绪
来源：http://hz.jyoumei.cn/gtosmzfohf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj20258.top/gtuofligec.html

[R73] 分割大日志
来源：http://hz.shanyushiyangkeji.top/gtocehioym.html

split -l 1000 big.log part_
来源：http://hz.tanke756.top/gtqhhnrshb.html

[R74] 批量重命名
来源：http://hz.chenlongwang.top/gtobbefayn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guannengcc.top/gtvnvelwxs.html

[R75] 导出环境变量
来源：http://hz.zdqjudy.top/gtttjtkwhu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ehwqpu.com/gtzamxzvmq.html

[R76] 使用临时文件
来源：http://hz.xuetiantiany.cn/gtodmcxaah.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtiwpevykl.html

[R77] 读取用户输入
来源：http://hz.birdmap.top/gtckccecsc.html

read -rp "请输入: " ans
来源：http://hz.tanke756.top/gtnrljlnpb.html

[R78] 交互式菜单
来源：http://hz.haohaochexian.top/gtkjwcvjwd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.aibaodan.cn/gtnfqgyszw.html

[R79] 解析命令行选项
来源：http://hz.zhaomingkeji.xyz/gtmoisppyg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtalfvammt.html

[R80] 查看脚本执行耗时
来源：http://hz.pengpengdd.cyou/gtizesxlmp.html

time ./run.sh
来源：http://hz.yj20258.top/gtmdsokitc.html

================================================================================
来源：http://hz.jinqigufen.top/gtyezjjcyx.html

S. C / C++ 专题
来源：http://hz.xingfuxueyuan.xyz/gtmejjfxst.html

================================================================================
来源：http://hz.yangfankeji.com/gtfyouxsdw.html

[S01] C：Hello World
来源：http://hz.nanxinkj.top/gtccdrudgl.html

#include <stdio.h>
来源：http://hz.vqdsnc.cn/gttccgwiaq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ppjwa.cn/gtasctopii.html

[S02] C：变量与格式化输出
来源：http://hz.wangdashe.top/gtogjbviqh.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhongyouzk.top/gtbununwyf.html

[S03] C：读入整数
来源：http://hz.shuidangran.top/gttlqnhcbx.html

int x; scanf("%d", &x);
来源：http://hz.yj20258888.top/gttqdooawc.html

[S04] C：字符串复制
来源：http://hz.zhixingplan.top/gtlwnvajkc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.pycfn.com/gtobawtxnn.html

[S05] C：字符串长度
来源：http://hz.gzhubu.top/gtmtcjozcx.html

strlen(s)
来源：http://hz.smart0.xyz/gttnlfcmkm.html

[S06] C：字符串比较
来源：http://hz.yueranfly.top/gtcjoooebv.html

strcmp(a, b) == 0
来源：http://hz.xingfuxueyuan.xyz/gtgkclzdnq.html

[S07] C：数组遍历求和
来源：http://hz.jyoumei.cn/gttrjhdkcq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuetiantiany.cn/gtlccwpcxr.html

[S08] C：动态内存分配与释放
来源：http://hz.pycfn.com/gtakdorqeo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cucudq.cn/gtcipjmjee.html

[S09] C：结构体定义与初始化
来源：http://hz.snrcjt.cn/gtsvkidsra.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fzhhl.top/gtlyxwiahp.html

[S10] C：指针与解引用
来源：http://hz.dianchejie.cn/gtnuqszdlv.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtcdfpdbml.html

[S11] C：逐行读文件
来源：http://hz.gogol.net.cn/gtrmrlhzuo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.daria6918.cn/gthpzudmhd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sxryk.cn/gtxscwwhys.html

fclose(f);
来源：http://hz.yvedp.cn/gtkdzbipsg.html

[S12] C：写文件
来源：http://hz.zhijiandao.cn/gtlhbddqwv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shanyushiyangtech.top/gtzhydprwz.html

[S13] C：宏定义
来源：http://hz.feifeiyinyue.top/gtakaqorcc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtlftwkqtq.html

[S14] C：枚举
来源：http://hz.cucudq.cn/gttxmjxhrv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pycfn.com/gtluflvfsd.html

[S15] C：类型转换
来源：http://hz.jlsjyb.cn/gtqjfocfrl.html

(double) a / b
来源：http://hz.chenzaomai.com/gtwsitokhv.html

[S16] C：位操作置位
来源：http://hz.ywan-chungtsiang.top/gtgbsmxybo.html

x |= (1 << 3);
来源：http://hz.gotoacloud.top/gtacxghykn.html

[S17] C：安全拼接字符串
来源：http://hz.hfpthk.cn/gtcovuxjju.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ydzc1.top/gtvpmjwxqd.html

[S18] C：命令行参数
来源：http://hz.9152youxi.cn/gtegvngutk.html

int main(int argc, char **argv)
来源：http://hz.gaohongyu789.top/gtvwgdcbru.html

[S19] C：快速排序
来源：http://hz.xuetiantiany.cn/gtpexqzaov.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtbjqnyvsl.html

[S20] C：二分查找
来源：http://hz.ehwqpu.com/gtmklmxqds.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenzaomai.com/gtbpqxsjql.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gtpjucvwqo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zdqjudy.top/gtabystuch.html

[S22] C：字符串转数字
来源：http://hz.guowangkeji.top/gteapoertk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.316326.xyz/gtjxvzkeav.html

[S23] C：随机数
来源：http://hz.dashuyun.cn/gtxocwuiwz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinghuilouyu.cn/gtlxkjoqjv.html

[S24] C：获取本地时间
来源：http://hz.wangdashe.top/gtbpofzkor.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hysaishi.cn/gtfbgkditl.html

[S25] C：内存拷贝
来源：http://hz.xylfe.cn/gtvqouzwdk.html

memcpy(dst, src, n);
来源：http://hz.jinghuilouyu.cn/gtpyipkdzu.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gtvfgtzuok.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258888.top/gtectgxusp.html

[S27] C：定义常量
来源：http://hz.wangshuangyany.cn/gtxzmpntnu.html

const double PI = 3.14159;
来源：http://hz.ybcxt.top/gtpxopwouf.html

[S28] C：静态变量
来源：http://hz.ehwqpu.com/gtrywlxbdh.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gtplwzomgw.html

[S29] C：变参函数
来源：http://hz.andypj.xyz/gtfonegmpo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.52xcode.cn/gtdgzcdxfj.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtedbtkvjh.html

#ifndef X_H
来源：http://hz.gogol.net.cn/gtgdngulzg.html

#define X_H
来源：http://hz.daxiang520.top/gtjyczdayc.html

#endif
来源：http://hz.ivvv.top/gtpnuanzzb.html

[S31] C++：Hello World
来源：http://hz.9152youxi.cn/gtbnejtfkl.html

#include <iostream>
来源：http://hz.dianchejie.cn/gtryptwcjl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tianlin.xyz/gtsziavnwc.html

[S32] C++：字符串
来源：http://hz.ybcxt.top/gtlcfdlara.html

std::string s = "hi";  s += "!";
来源：http://hz.yangfankeji.com/gtztsjqhnt.html

[S33] C++：vector 增删
来源：http://hz.haohaochexian.top/gtfgjerqzb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gttxhgwutx.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gttcisftge.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hfpthk.cn/gtrdnkwreh.html

[S35] C++：map
来源：http://hz.xuetiantiany.cn/gtdaxbaryl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.snrcjt.cn/gtimcaiiet.html

[S36] C++：unordered_map
来源：http://hz.zycfv.cn/gtjcvnemny.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtafvejvbn.html

[S37] C++：set
来源：http://hz.wangshuangyany.cn/gtxuozhwbl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yj20258.top/gtpwsurdfg.html

[S38] C++：排序
来源：http://hz.dashuyun.cn/gtzvknqpgq.html

std::sort(v.begin(), v.end());
来源：http://hz.ivvv.top/gtxtuborti.html

[S39] C++：自定义比较器排序
来源：http://hz.52xcode.cn/gttpzbwrby.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gaohongyu789.top/gtkqjeomdd.html

[S40] C++：查找元素
来源：http://hz.gaohongyu789.top/gtgfsqiwyn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gaohongyu789.top/gtlgnlrkgh.html

[S41] C++：类与构造函数
来源：http://hz.zycfv.cn/gtxjcstjbt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guannengcc.top/gtaeijatpo.html

[S42] C++：继承与虚函数
来源：http://hz.yuanzhike.top/gtxnxldbbl.html

class B : public Base { public: void f() override {} };
来源：http://hz.bjfxy.top/gtbvghjshr.html

[S43] C++：智能指针
来源：http://hz.yanxiufei.cn/gtfomhqxzh.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuxming.cn/gtynkstbdv.html

[S44] C++：引用传参
来源：http://hz.shzxlz.cn/gtkzndjetf.html

void inc(int &x) { ++x; }
来源：http://hz.xinyue.icu/gtdeofykmv.html

[S45] C++：lambda
来源：http://hz.cashguo.top/gtmsrqhhon.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhijiandao.cn/gtbnluplze.html

[S46] C++：函数模板
来源：http://hz.cucudq.cn/gtnrqlvmim.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj202588.top/gtsswujgya.html

[S47] C++：结构化绑定遍历
来源：http://hz.svipenyu.cn/gtrdrwuape.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zycfv.cn/gtgjhgzhjt.html

[S48] C++：逐行读文件
来源：http://hz.chenzaomai.com/gtvrabfnwq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hfpthk.cn/gtnkojzosq.html

while (std::getline(in, line)) { }
来源：http://hz.sweek.top/gtsppnzsvf.html

[S49] C++：写文件
来源：http://hz.smart0.xyz/gtairxjtwt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jianghu66.top/gtvuzjkutk.html

[S50] C++：格式化数字
来源：http://hz.birdmap.top/gtdwqapdvz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zdqjudy.top/gttgmeepog.html

[S51] C++：显式类型转换
来源：http://hz.pycfn.com/gtxhdoblgq.html

static_cast<double>(a) / b
来源：http://hz.kuanghao11.cn/gtxqufiaoz.html

[S52] C++：const 与 noexcept
来源：http://hz.gaohongyu789.top/gtgzsqqldn.html

int size() const noexcept { return n_; }
来源：http://hz.iojbl.cn/gtosqmvvsj.html

[S53] C++：移动语义
来源：http://hz.havefunace.top/gtaiuuswzg.html

std::vector<int> w = std::move(v);
来源：http://hz.xziqi.cn/gthgbdlzrk.html

[S54] C++：异常处理
来源：http://hz.redwolf501.top/gtpxwvjgpd.html


<!-- 参考信息 -->