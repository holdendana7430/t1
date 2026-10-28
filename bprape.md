代发 wailian999

[Q76] 按天统计
来源：http://hz.zhixingplan.top/gtuyqqdfen.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.52xcode.cn/gtidbkmosm.html

[Q77] 时间加减
来源：http://hz.snrcjt.cn/gtfrhsqula.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.dashuyun.cn/gtjmrrrgxn.html

[Q78] 当前时间
来源：http://hz.chenlongwang.top/gttrcyjnrg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuxming.cn/gtolrvjwfn.html

[Q79] 字符串拼接
来源：http://hz.zhiwuduotai.top/gtcuqhyjtc.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.52xcode.cn/gtgjoevmeq.html

[Q80] 字符串截取
来源：http://hz.zhijiandao.cn/gtfuzkdtls.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hywenlv.cn/gtsplldjyu.html

[Q81] 字符串替换
来源：http://hz.xuanzx.com/gtfjugmwjz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgfzy.top/gtjssejdwv.html

[Q82] 字符长度与字节长度
来源：http://hz.ehwqpu.com/gtdcvelxog.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gthengxgzw.html

[Q83] 大小写转换
来源：http://hz.wangdashe.top/gtyrrsnkwh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj202588.top/gtipxourrb.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gttazbashb.html

SELECT TRIM(name) FROM users;
来源：http://hz.ppjwa.cn/gtqjbrntbz.html

[Q85] 数值取整
来源：http://hz.hfpthk.cn/gtlzcreydl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yonumen.top/gtylqdybfy.html

[Q86] 读取 JSON 字段
来源：http://hz.jinqigfzy.top/gtlihkpohl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhiwuduotai.top/gtyjoninan.html

[Q87] JSON 字段做条件
来源：http://hz.cqqwz.cn/gtciahibum.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xingfuxueyuan.xyz/gtvrwyiasl.html

[Q88] 行转列（条件聚合）
来源：http://hz.dashuyun.cn/gtdeieqtkx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hnxiangtu.top/gtexytaigm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.feifeiyinyue.top/gtaxsgbdqt.html

[Q89] 判断表是否存在
来源：http://hz.shuidangran.top/gthxrzjgiw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xingfuxueyuan.xyz/gtzphgwhvt.html

[Q90] 生成序号列
来源：http://hz.chenlongwang.top/gtsxzzgrgf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hammf.cn/gtkwdyqgji.html

================================================================================
来源：http://hz.chenlongwang.top/gtjcsynqun.html

R. Bash 专题
来源：http://hz.nanxuanxn.top/gtqwvnjmtj.html

================================================================================
来源：http://hz.andypj.xyz/gttysllgcr.html

[R01] shebang 与严格模式
来源：http://hz.zhaomingkeji.xyz/gtxqcauwmy.html

#!/usr/bin/env bash
来源：http://hz.fengsongda.top/gtkjeobsne.html

set -euo pipefail
来源：http://hz.fzhhl.top/gtybbzsspo.html

[R02] 变量赋值与使用
来源：http://hz.hongshengwenyu.top/gtigrxdaoy.html

name="Tom"; echo "$name"
来源：http://hz.ivvv.top/gtwdfpnjvx.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gtvrbnbvmt.html

readonly PI=3.14
来源：http://hz.hysaishi.cn/gthhkjalwa.html

[R04] 位置参数
来源：http://hz.hfpthk.cn/gtattjywdt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ywan-chungtsiang.top/gtzfvclfhg.html

[R05] 参数默认值
来源：http://hz.hongshengwenyu.top/gtftcujobh.html

name="${1:-default}"
来源：http://hz.zhijiandao.cn/gtunuvwgag.html

[R06] 判断命令是否存在
来源：http://hz.daria6918.cn/gtnqpidsfu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.haohaochexian.top/gtepmcgowg.html

[R07] if 判断文件
来源：http://hz.guowangkeji.top/gtylhkizqx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.aizwys.cn/gtyhzmkcxe.html

[R08] 数值比较
来源：http://hz.yanxiufei.cn/gtgxcaqfho.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.birdmap.top/gttoscvcsj.html

[R09] 字符串比较
来源：http://hz.svipenyu.cn/gtgoschsag.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.meibo888.top/gtzpvmtors.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gtrvoxyaxa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.quarkkingdee.top/gtqjvehgml.html

[R11] case 多分支
来源：http://hz.havefunace.top/gtfrnfamic.html

case "$1" in
来源：http://hz.andypj.xyz/gtgqbezoju.html

start) echo "启动" ;;
来源：http://hz.sweek.top/gtduvatzbg.html

stop)  echo "停止" ;;
来源：http://hz.zhixingplan.top/gtonuhnctm.html

*)     echo "未知命令" ;;
来源：http://hz.xuanzx.com/gtwalgndjs.html

esac
来源：http://hz.chenzaomai.com/gtjewcjxui.html

[R12] for 遍历文件
来源：http://hz.nanxuanxn.top/gtoiuxxtub.html

for f in *.txt; do echo "$f"; done
来源：http://hz.smart0.xyz/gtvbontxwx.html

[R13] for 计数循环
来源：http://hz.pengpengdd.cyou/gtovmwzlpn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gogol.net.cn/gtzccbfhet.html

[R14] C 风格 for
来源：http://hz.9152youxi.cn/gtukqtmeaa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dianchejie.cn/gtotkavpia.html

[R15] while 逐行读文件
来源：http://hz.dianchejie.cn/gtjzvjdmrl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zycfv.cn/gtotkgydux.html

[R16] until 等待条件
来源：http://hz.fengsongda.top/gtwgesqdnx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cucudq.cn/gthxzsybji.html

[R17] 数组定义与取值
来源：http://hz.yonumen.top/gtjapkcwkm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.fzhhl.top/gtqmedtjdm.html

[R18] 遍历数组
来源：http://hz.tianlin.xyz/gtukbncqun.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuanzhike.top/gtrbzgnhyj.html

[R19] 数组长度
来源：http://hz.zhiwuduotai.top/gtcbibcxue.html

echo "${#arr[@]}"
来源：http://hz.zhixingplan.top/gtlveylwyi.html

[R20] 关联数组（字典）
来源：http://hz.fzhhl.top/gtfmrxxaaz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yuxming.cn/gttmawsqrf.html

[R21] 字符串长度
来源：http://hz.meibo888.top/gtvmsxpofe.html

echo "${#s}"
来源：http://hz.shanyushiyangkeji.top/gtydcnznjf.html

[R22] 截取子串
来源：http://hz.hysaishi.cn/gttstrkibp.html

echo "${s:0:5}"
来源：http://hz.gaohongyu789.top/gtaexlfxsr.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gtjougezkl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shuidangran.top/gthvrsbfni.html

[R24] 大小写转换
来源：http://hz.ydjk.org.cn/gtwiuhvisu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jyoumei.cn/gtfcibwvve.html

[R25] 去后缀 / 去前缀
来源：http://hz.xingfuxueyuan.xyz/gttiaquhqo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.haohaochexian.top/gtrvsugkrp.html

[R26] 命令替换
来源：http://hz.dianchejie.cn/gtcowderyh.html

now=$(date +%F); echo "$now"
来源：http://hz.yj202588.top/gtddkfdagn.html

[R27] 算术展开
来源：http://hz.zhiwuduotai.top/gtsbomyrnu.html

echo $((1 + 2 * 3))
来源：http://hz.yuanzhike.top/gtcsqcjrxf.html

[R28] 浮点运算
来源：http://hz.redwolf501.top/gtilswrlak.html

echo "scale=2; 10/3" | bc
来源：http://hz.316326.xyz/gtoraexspb.html

[R29] 定义函数
来源：http://hz.ehwqpu.com/gteolanhku.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jyoumei.cn/gtinanzzqm.html

[R30] 函数返回状态码
来源：http://hz.xziqi.cn/gtolgnghhw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtfsftcvfu.html

[R31] 局部变量
来源：http://hz.yj20258888.top/gtqpyfjaoz.html

f() { local x=1; echo "$x"; }
来源：http://hz.fengsongda.top/gtcydiljgb.html

[R32] 参数个数校验
来源：http://hz.nwbrower.top/gtiufeybyg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sweek.top/gtmpepplct.html

[R33] 捕获错误并提示行号
来源：http://hz.xuetiantiany.cn/gtvchgryzm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.iojbl.cn/gtutmgdkwi.html

[R34] 退出时清理
来源：http://hz.zhaomingkeji.xyz/gtsqviyjxp.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtpjjlabou.html

[R35] 后台执行并等待
来源：http://hz.c1oappe.top/gtczddpeml.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtamuisyfn.html

[R36] 并发执行多个任务
来源：http://hz.bjfxy.top/gtsxbcjkgs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cheryme.top/gtyucsjczu.html

[R37] 把输出赋给变量
来源：http://hz.vqdsnc.cn/gtiywkrxjy.html

files=$(ls -1)
来源：http://hz.daria6918.cn/gtvtpkpxkb.html

[R38] 管道串联
来源：http://hz.cucudq.cn/gtlyxeiypw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cqqwz.cn/gtlmmqitrp.html

[R39] 重定向标准输出与错误
来源：http://hz.ydjk.org.cn/gtmrpjcfri.html

cmd > out.log 2>&1
来源：http://hz.jianghu66.top/gtwyetqwmx.html

[R40] 追加写日志
来源：http://hz.9152youxi.cn/gturmcnmya.html

echo "log" >> out.log
来源：http://hz.tanke756.top/gtyanafvxo.html

[R41] 丢弃输出
来源：http://hz.guannengcc.top/gtbrextmmh.html

cmd >/dev/null 2>&1
来源：http://hz.yvedp.cn/gtfgojkjnt.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gtozaijibj.html

wc -l < a.txt
来源：http://hz.zhengqikj.top/gtlsacrpin.html

[R43] 按名字查找文件
来源：http://hz.shanyushiyangtech.top/gtyhaslmvx.html

find . -name "*.log" -type f
来源：http://hz.shangyingyoupin.top/gtarhynzwf.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gtowbzhhso.html

find . -mtime -7 -type f
来源：http://hz.birdmap.top/gtkihyqdfx.html

[R45] 批量删除
来源：http://hz.cqqwz.cn/gttzlgtequ.html

find . -name "*.tmp" -delete
来源：http://hz.snrcjt.cn/gtceonnagk.html

[R46] 递归替换文件内容
来源：http://hz.pengpengdd.cyou/gthvoexhrp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ehwqpu.com/gtbebdxgcb.html

[R47] sed 单行替换
来源：http://hz.hongshengwenyu.top/gtandswpoy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hfpthk.cn/gtfornyexp.html

[R48] awk 取指定列
来源：http://hz.nwbrower.top/gtimwiexkv.html

awk '{print $1, $3}' a.txt
来源：http://hz.yuanzhike.top/gtecpfreem.html

[R49] awk 带条件
来源：http://hz.xuanzx.com/gticwywyvf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj202588.top/gtdvwslmtp.html

[R50] awk 求和
来源：http://hz.shuidangran.top/gthcrvamrw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dianchejie.cn/gtxzqxyqwz.html

[R51] 排序去重取前几
来源：http://hz.aizwys.cn/gtgdjruqsa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tian-w.cn/gtildbyfzi.html

[R52] 统计行数
来源：http://hz.ybcxt.top/gtwshvcesc.html

wc -l a.txt
来源：http://hz.cashguo.top/gtaaiawoce.html

[R53] 查看文件头与实时尾
来源：http://hz.jiagoushi.top/gtqovxrxdk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenjidiqi.icu/gtrzyuzjqs.html

[R54] 比较两个文件
来源：http://hz.52xcode.cn/gttyrjfjyo.html

diff a.txt b.txt
来源：http://hz.birdmap.top/gtvikkvewd.html

[R55] 压缩与解压
来源：http://hz.bjfxy.top/gtppvdezdp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.iojbl.cn/gtfwywafjs.html

[R56] 远程拷贝
来源：http://hz.jqgufenzy.top/gtenkrwamp.html

scp file user@host:/path/
来源：http://hz.cheryme.top/gtoffcugwi.html

[R57] 远程执行命令
来源：http://hz.jyoumei.cn/gtxjxnjjvj.html

ssh user@host 'uptime'
来源：http://hz.yueranfly.top/gtqdzupdhe.html

[R58] 下载文件
来源：http://hz.xuetiantiany.cn/gthgrfafhp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pycfn.com/gtxrpkthrr.html

[R59] 发 POST JSON
来源：http://hz.52xcode.cn/gtmblyblyl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxuanxn.top/gtqfdydhga.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhengqikj.top/gtlkxjovgd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gotoacloud.top/gtjigxtcmr.html

[R61] 磁盘占用
来源：http://hz.wangshuangyany.cn/gtrfoqxsmr.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gtnjopcfjd.html

[R62] 找最占空间的文件
来源：http://hz.tianlin.xyz/gtjpwvteoe.html

du -ah . | sort -rh | head -10
来源：http://hz.xziqi.cn/gtsnlynpxc.html

[R63] 内存与进程
来源：http://hz.shuidangran.top/gtdntmmset.html

free -h;  ps aux | grep nginx
来源：http://hz.9152youxi.cn/gtdispeqfq.html

[R64] 结束进程
来源：http://hz.quarkkingdee.top/gtkwvexiyp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hongshengwenyu.top/gtlhpwodyr.html

[R65] 查看端口占用
来源：http://hz.guannengcc.top/gtranazenf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.quarkkingdee.top/gtrxjtoraq.html

[R66] 定时任务
来源：http://hz.havefunace.top/gtzkyhiawg.html

crontab -e;  crontab -l
来源：http://hz.guannengcc.top/gtjuhhwimk.html

[R67] 生成随机十六进制串
来源：http://hz.xylfe.cn/gtyufpmhex.html

openssl rand -hex 16
来源：http://hz.smart0.xyz/gtbkhqpayu.html

[R68] 计算文件校验值
来源：http://hz.zhongyouzk.top/gtjezliefx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ppjwa.cn/gtnhoyejlg.html

[R69] 生成随机密码
来源：http://hz.yj20258.top/gtsxdbytqq.html

head -c 16 /dev/urandom | base64
来源：http://hz.zdqjudy.top/gtwimjpuey.html

[R70] 时间戳与互转
来源：http://hz.xuanzx.com/gtjnycwgol.html

date +%s;  date -d @1700000000
来源：http://hz.aizwys.cn/gtmmogjnac.html

[R71] 日期格式化
来源：http://hz.tian-w.cn/gtltbkwkkf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxuanxn.top/gtchszkhve.html

[R72] 等待端口就绪
来源：http://hz.hfpthk.cn/gtxfjwwqub.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigufen.top/gtghhaahez.html

[R73] 分割大日志
来源：http://hz.jinghuilouyu.cn/gtsanjwmki.html

split -l 1000 big.log part_
来源：http://hz.316326.xyz/gtwozreigf.html

[R74] 批量重命名
来源：http://hz.zhongyouzk.top/gtzwfoijfa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xziqi.cn/gtvtahipxs.html

[R75] 导出环境变量
来源：http://hz.yonumen.top/gtyqgaralx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shuidangran.top/gtlbshobrl.html

[R76] 使用临时文件
来源：http://hz.birdmap.top/gtujrvebvb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sysykeji.top/gthbhastye.html

[R77] 读取用户输入
来源：http://hz.zhixingplan.top/gteiosjwof.html

read -rp "请输入: " ans
来源：http://hz.hnqzz.top/gtsfuhmyrf.html

[R78] 交互式菜单
来源：http://hz.feifeiyinyue.top/gtezrdrivy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yanxiufei.cn/gtpisegjmm.html

[R79] 解析命令行选项
来源：http://hz.xuetiantiany.cn/gtygpgbcpc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtfvejdpnk.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtobnbysww.html

time ./run.sh
来源：http://hz.chenzaomai.com/gtdzjhfstb.html

================================================================================
来源：http://hz.fengsongda.top/gtfoyzqiny.html

S. C / C++ 专题
来源：http://hz.xziqi.cn/gtftuhnbdj.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtifzsyivq.html

[S01] C：Hello World
来源：http://hz.hysaishi.cn/gtazguiero.html

#include <stdio.h>
来源：http://hz.xinyue.icu/gtmkkjqxku.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jlsjyb.cn/gtiamvgnqx.html

[S02] C：变量与格式化输出
来源：http://hz.fzhhl.top/gtjhzaumkz.html

int a = 10; printf("%d\n", a);
来源：http://hz.dashuyun.cn/gtirsrxwss.html

[S03] C：读入整数
来源：http://hz.nwbrower.top/gtgaeiwaqk.html

int x; scanf("%d", &x);
来源：http://hz.pengpengdd.cyou/gtcmebizga.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangtech.top/gtlfborpvy.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.sxryk.cn/gtvlininsx.html

[S05] C：字符串长度
来源：http://hz.daria6918.cn/gtggdfsjsw.html

strlen(s)
来源：http://hz.jinqigfzy.top/gtorgghrrl.html

[S06] C：字符串比较
来源：http://hz.yuxming.cn/gtbkmhgtqf.html

strcmp(a, b) == 0
来源：http://hz.pengpengdd.cyou/gtadlaiimo.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangtech.top/gtlcqyfpfn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shzxlz.cn/gtmfctmbke.html

[S08] C：动态内存分配与释放
来源：http://hz.yueranfly.top/gtjzoczcjn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daria6918.cn/gtdcvaexlk.html

[S09] C：结构体定义与初始化
来源：http://hz.fengsongda.top/gtnofnopoc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yonumen.top/gtyemykjdp.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtzjntuikk.html

int *p = &a;  *p = 5;
来源：http://hz.hammf.cn/gtytdpfmbr.html

[S11] C：逐行读文件
来源：http://hz.chenlongwang.top/gtpwfjwhot.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sxryk.cn/gtpaivbsez.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.smart0.xyz/gtkldpctwg.html

fclose(f);
来源：http://hz.cucudq.cn/gthmfldbru.html

[S12] C：写文件
来源：http://hz.iojbl.cn/gtthykmrtz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cqqwz.cn/gtbxtrtkxm.html

[S13] C：宏定义
来源：http://hz.gaohongyu789.top/gthgywhldd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ppjwa.cn/gtokooczyo.html

[S14] C：枚举
来源：http://hz.zhiwuduotai.top/gtmmyktutf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhoulong.xyz/gtamuoemwq.html

[S15] C：类型转换
来源：http://hz.ehwqpu.com/gtzzcxrhph.html

(double) a / b
来源：http://hz.sufxvd.cn/gtyreovgcx.html

[S16] C：位操作置位
来源：http://hz.snrcjt.cn/gtejjdvrlk.html

x |= (1 << 3);
来源：http://hz.dashuyun.cn/gthwisjilh.html

[S17] C：安全拼接字符串
来源：http://hz.0kj1m.cn/gtaikyxszv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zdqjudy.top/gtejzvxlvz.html

[S18] C：命令行参数
来源：http://hz.ydjk.org.cn/gtkdtibnhg.html

int main(int argc, char **argv)
来源：http://hz.sweek.top/gtkptllmxf.html

[S19] C：快速排序
来源：http://hz.ehwqpu.com/gtrfebejkr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtytsoclfk.html

[S20] C：二分查找
来源：http://hz.shanyushiyangtech.top/gtrjbuavza.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhoulong.xyz/gtqkadioiq.html

[S21] C：字符类别判断
来源：http://hz.nanxinkj.top/gtfrauwdsf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pengpengdd.cyou/gtewwqjafo.html

[S22] C：字符串转数字
来源：http://hz.jinyuanbaomall.cn/gtmfblzbaa.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuanzhike.top/gthtkmqtcz.html

[S23] C：随机数
来源：http://hz.vqdsnc.cn/gtuzjoprzn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daria6918.cn/gtbjjhshlk.html

[S24] C：获取本地时间
来源：http://hz.316326.xyz/gtaryfjazn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtgeplnfwg.html

[S25] C：内存拷贝
来源：http://hz.ydzc1.top/gtxqyvkdyo.html

memcpy(dst, src, n);
来源：http://hz.guowangkeji.top/gtwbdojgel.html

[S26] C：内存清零
来源：http://hz.zhiwuduotai.top/gtmqndiogj.html

memset(a, 0, sizeof a);
来源：http://hz.gzhubu.top/gtserpgsbb.html

[S27] C：定义常量
来源：http://hz.cashguo.top/gtucjnjmuk.html

const double PI = 3.14159;
来源：http://hz.c1oappe.top/gtoybjyidx.html

[S28] C：静态变量
来源：http://hz.cucudq.cn/gtiihgbnbn.html

static int counter = 0;
来源：http://hz.shzxlz.cn/gtkysvnsdx.html

[S29] C：变参函数
来源：http://hz.havefunace.top/gtmuimamqy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daxiang520.top/gtifsnlljx.html

[S30] C：头文件保护
来源：http://hz.hywenlv.cn/gtdbnkwkxu.html

#ifndef X_H
来源：http://hz.0kj1m.cn/gtvleyvalq.html

#define X_H
来源：http://hz.316326.xyz/gteoodqoxk.html

#endif
来源：http://hz.yj20258888.top/gtdijdtgyh.html

[S31] C++：Hello World
来源：http://hz.bjfxy.top/gtlbvkfwiw.html

#include <iostream>
来源：http://hz.birdmap.top/gtwxenxnpy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.vqdsnc.cn/gtzdakwjbn.html

[S32] C++：字符串
来源：http://hz.daxiang520.top/gtjexbtbth.html

std::string s = "hi";  s += "!";
来源：http://hz.fengsongda.top/gthrvatbkc.html

[S33] C++：vector 增删
来源：http://hz.quarkkingdee.top/gtrxywqqfb.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zycfv.cn/gtnypvdspl.html

[S34] C++：遍历 vector
来源：http://hz.hammf.cn/gtvkfdfwaz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jyoumei.cn/gtrwtlbzls.html

[S35] C++：map
来源：http://hz.yvedp.cn/gtnjghrpfj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnxiangtu.top/gtuttmfxvy.html

[S36] C++：unordered_map
来源：http://hz.daxiang520.top/gtcpnxznga.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.mhx1999.top/gtvowfvgao.html

[S37] C++：set
来源：http://hz.jianghu66.top/gtrmlbeuzo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhijiandao.cn/gtidyiecye.html

[S38] C++：排序
来源：http://hz.hywenlv.cn/gtmtczzulr.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgufenzy.top/gtgzsqghol.html

[S39] C++：自定义比较器排序
来源：http://hz.snrcjt.cn/gtulrkjwpq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.nanxuanxn.top/gtzcrhvdbg.html

[S40] C++：查找元素
来源：http://hz.cdnleiting.top/gtxwofyuet.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hnxiangtu.top/gtemusrewt.html

[S41] C++：类与构造函数
来源：http://hz.shzxlz.cn/gtrhbgpiag.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.redwolf501.top/gteizwvxmu.html

[S42] C++：继承与虚函数
来源：http://hz.ywan-chungtsiang.top/gtsxrevzfh.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtpegqoxkj.html

[S43] C++：智能指针
来源：http://hz.shuidangran.top/gtsqxmllck.html

auto p = std::make_unique<int>(5);
来源：http://hz.kuanghao11.cn/gthizeocqj.html

[S44] C++：引用传参
来源：http://hz.xinyue.icu/gtqpbziwqq.html

void inc(int &x) { ++x; }
来源：http://hz.nanxinkj.top/gtzkyeyref.html

[S45] C++：lambda
来源：http://hz.guannengcc.top/gttpbksghx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.c1oappe.top/gtjjcnqrjn.html

[S46] C++：函数模板
来源：http://hz.hywenlv.cn/gtmevwmeih.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gtidloleei.html


<!-- 参考信息 -->