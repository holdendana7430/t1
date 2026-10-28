代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jyoumei.cn/gtohudmzpc.html

[Q75] 日期格式化
来源：http://hz.jiagoushi.top/gtiwkoamug.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cucudq.cn/gteflbknma.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ybcxt.top/gtcrkyhqoh.html

[Q76] 按天统计
来源：http://hz.zhixingplan.top/gteubnteqi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tian-w.cn/gtjbgjuxui.html

[Q77] 时间加减
来源：http://hz.feifeiyinyue.top/gtrusysvge.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhaomingkeji.xyz/gtbrqcgaox.html

[Q78] 当前时间
来源：http://hz.wangshuangyany.cn/gtmoayfurm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xuetiantiany.cn/gtrplxvcbk.html

[Q79] 字符串拼接
来源：http://hz.nwbrower.top/gtohjlbqsi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daxiang520.top/gtschbxkpa.html

[Q80] 字符串截取
来源：http://hz.guowangkeji.top/gtancrjykq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydzc1.top/gtuqfulavi.html

[Q81] 字符串替换
来源：http://hz.cheryme.top/gtonxqemvp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.daxiang520.top/gtbboeejpj.html

[Q82] 字符长度与字节长度
来源：http://hz.jinqigfzy.top/gtgtwbzgui.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gtyzygmepx.html

[Q83] 大小写转换
来源：http://hz.cqqwz.cn/gtoohqxaqp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxinkj.top/gtdrknemnp.html

[Q84] 去除首尾空格
来源：http://hz.9152youxi.cn/gtnpvdhbdz.html

SELECT TRIM(name) FROM users;
来源：http://hz.mhx1999.top/gtezpgcxiq.html

[Q85] 数值取整
来源：http://hz.yueranfly.top/gthdwcqide.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.quarkkingdee.top/gtxtnjofdb.html

[Q86] 读取 JSON 字段
来源：http://hz.cucudq.cn/gttqbkqnnl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gotoacloud.top/gtlrjwkupk.html

[Q87] JSON 字段做条件
来源：http://hz.jiagoushi.top/gtsunsadmc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenlongwang.top/gtgxacokey.html

[Q88] 行转列（条件聚合）
来源：http://hz.snrcjt.cn/gtzvyvknoo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.aizwys.cn/gtlnegvqjr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.andypj.xyz/gtxkondqjq.html

[Q89] 判断表是否存在
来源：http://hz.meibo888.top/gtmjakttqx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hysaishi.cn/gtnraxdcrb.html

[Q90] 生成序号列
来源：http://hz.yueranfly.top/gtshjubooy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenzaomai.com/gtolvyfasj.html

================================================================================
来源：http://hz.sxryk.cn/gtzgxcirya.html

R. Bash 专题
来源：http://hz.xylfe.cn/gtnujmnuif.html

================================================================================
来源：http://hz.cheryme.top/gtdfefpacz.html

[R01] shebang 与严格模式
来源：http://hz.dashuyun.cn/gtdoapqsfk.html

#!/usr/bin/env bash
来源：http://hz.tian-w.cn/gtqwjbixpl.html

set -euo pipefail
来源：http://hz.yonumen.top/gtwruibjnr.html

[R02] 变量赋值与使用
来源：http://hz.sysykeji.top/gtjycrajse.html

name="Tom"; echo "$name"
来源：http://hz.chenzaomai.com/gtoxjspbqt.html

[R03] 只读变量
来源：http://hz.yvedp.cn/gthityseqw.html

readonly PI=3.14
来源：http://hz.9152youxi.cn/gtegphunvj.html

[R04] 位置参数
来源：http://hz.shanyushiyangtech.top/gtelqrzsad.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.c1oappe.top/gtukjbejim.html

[R05] 参数默认值
来源：http://hz.c1oappe.top/gtvlpaexdd.html

name="${1:-default}"
来源：http://hz.sxryk.cn/gtojqawzak.html

[R06] 判断命令是否存在
来源：http://hz.feifeiyinyue.top/gtlvvsckli.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shuidangran.top/gtmrletobm.html

[R07] if 判断文件
来源：http://hz.fengsongda.top/gtkljljyco.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.andypj.xyz/gtbterjuyd.html

[R08] 数值比较
来源：http://hz.zhongyouzk.top/gtfritsmqp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.vqdsnc.cn/gtyiwmeklt.html

[R09] 字符串比较
来源：http://hz.birdmap.top/gtjnsplqcn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gotoacloud.top/gtnpjhmtjz.html

[R10] 正则匹配
来源：http://hz.vqdsnc.cn/gtgwauyelx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj20258888.top/gtpxgopbjm.html

[R11] case 多分支
来源：http://hz.fzhhl.top/gtblmivbul.html

case "$1" in
来源：http://hz.hywenlv.cn/gtrzuevkff.html

start) echo "启动" ;;
来源：http://hz.daxiang520.top/gtccqmfgao.html

stop)  echo "停止" ;;
来源：http://hz.mhx1999.top/gtmferrfzz.html

*)     echo "未知命令" ;;
来源：http://hz.chenzaomai.com/gtjgqyzsra.html

esac
来源：http://hz.sysykeji.top/gtuplqotfl.html

[R12] for 遍历文件
来源：http://hz.redwolf501.top/gtocbwhzhh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtwznzmscd.html

[R13] for 计数循环
来源：http://hz.jinqigfzy.top/gtxwhrgdpw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhengqikj.top/gtaxldnuiv.html

[R14] C 风格 for
来源：http://hz.shuidangran.top/gtvwpnxnid.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yvedp.cn/gtcgaulxpy.html

[R15] while 逐行读文件
来源：http://hz.zhoulong.xyz/gtodgrldwx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gzhubu.top/gtsdkobfhh.html

[R16] until 等待条件
来源：http://hz.redwolf501.top/gtzsaxkvnu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangdashe.top/gtzailpqyd.html

[R17] 数组定义与取值
来源：http://hz.jinqigufen.top/gtyrkthrpi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xinyue.icu/gtmlslyotq.html

[R18] 遍历数组
来源：http://hz.snrcjt.cn/gtjcvlsfdo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guannengcc.top/gtzrqoigtv.html

[R19] 数组长度
来源：http://hz.ydjk.org.cn/gtqkiayimc.html

echo "${#arr[@]}"
来源：http://hz.jiagoushi.top/gtugjhbvtq.html

[R20] 关联数组（字典）
来源：http://hz.sweek.top/gteogtquhe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yvedp.cn/gtymnyftae.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtcadipcby.html

echo "${#s}"
来源：http://hz.yangfankeji.com/gtsceifjqn.html

[R22] 截取子串
来源：http://hz.ppjwa.cn/gtnjmkmqyj.html

echo "${s:0:5}"
来源：http://hz.quarkkingdee.top/gtodvzlxsa.html

[R23] 字符串替换
来源：http://hz.yuanzhike.top/gtvycyxels.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.smart0.xyz/gtoczylyiy.html

[R24] 大小写转换
来源：http://hz.yuxming.cn/gtckimibod.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sufxvd.cn/gtxabcivsq.html

[R25] 去后缀 / 去前缀
来源：http://hz.wangshuangyany.cn/gtckuwkghc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydjk.org.cn/gtqyybecjh.html

[R26] 命令替换
来源：http://hz.fengsongda.top/gtzurwinzm.html

now=$(date +%F); echo "$now"
来源：http://hz.cdnleiting.top/gtazmlvpur.html

[R27] 算术展开
来源：http://hz.dashuyun.cn/gtbxubzhjs.html

echo $((1 + 2 * 3))
来源：http://hz.jqgfzy.top/gteyrubdlr.html

[R28] 浮点运算
来源：http://hz.cucudq.cn/gtryjmxtrb.html

echo "scale=2; 10/3" | bc
来源：http://hz.xinyue.icu/gtdomlfdiy.html

[R29] 定义函数
来源：http://hz.cheryme.top/gtndjjeobv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258888.top/gtpzvqprut.html

[R30] 函数返回状态码
来源：http://hz.zycfv.cn/gtgbvrnooy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ydjk.org.cn/gthfcqogdb.html

[R31] 局部变量
来源：http://hz.mhx1999.top/gtkivorkvd.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydjk.org.cn/gtkjfgxcdz.html

[R32] 参数个数校验
来源：http://hz.nanxuanxn.top/gtpzvosckp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.guannengcc.top/gthabiovza.html

[R33] 捕获错误并提示行号
来源：http://hz.sxryk.cn/gtofmyyfbg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangtech.top/gtfpzlenly.html

[R34] 退出时清理
来源：http://hz.hammf.cn/gteovftsjg.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtsbvgmhdx.html

[R35] 后台执行并等待
来源：http://hz.kuanghao11.cn/gtxkqbmlcp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.aibaodan.cn/gtmozcfurl.html

[R36] 并发执行多个任务
来源：http://hz.jqgfzy.top/gteftvjvrc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.316326.xyz/gtdlkpvgbs.html

[R37] 把输出赋给变量
来源：http://hz.tianlin.xyz/gtbmtfiyak.html

files=$(ls -1)
来源：http://hz.sufxvd.cn/gtsciyunxb.html

[R38] 管道串联
来源：http://hz.jinyuanbaomall.cn/gtniqtkmbv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtchgbrbuk.html

[R39] 重定向标准输出与错误
来源：http://hz.gotoacloud.top/gtmmxqazcf.html

cmd > out.log 2>&1
来源：http://hz.jlsjyb.cn/gtallrarxg.html

[R40] 追加写日志
来源：http://hz.yuanzhike.top/gtidkzhrry.html

echo "log" >> out.log
来源：http://hz.chenlongwang.top/gtamgtecyv.html

[R41] 丢弃输出
来源：http://hz.smart0.xyz/gtearnpxha.html

cmd >/dev/null 2>&1
来源：http://hz.guannengcc.top/gtjezxrdch.html

[R42] 输入重定向
来源：http://hz.hammf.cn/gthikrwrze.html

wc -l < a.txt
来源：http://hz.c1oappe.top/gtvapgzyoe.html

[R43] 按名字查找文件
来源：http://hz.hnxiangtu.top/gtwgwiirmm.html

find . -name "*.log" -type f
来源：http://hz.pycfn.com/gthfahzqjm.html

[R44] 按修改时间查找
来源：http://hz.guannengcc.top/gtrvuqnfud.html

find . -mtime -7 -type f
来源：http://hz.0kj1m.cn/gtuwbjpurg.html

[R45] 批量删除
来源：http://hz.nanxuanxn.top/gtorumnfwz.html

find . -name "*.tmp" -delete
来源：http://hz.ivvv.top/gtfyhdbust.html

[R46] 递归替换文件内容
来源：http://hz.sufxvd.cn/gtiafqybgv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gaohongyu789.top/gtlgalwsos.html

[R47] sed 单行替换
来源：http://hz.yuxming.cn/gtzcmtumsx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yonumen.top/gtyfyscjfb.html

[R48] awk 取指定列
来源：http://hz.shanyushiyangkeji.top/gteelhqznj.html

awk '{print $1, $3}' a.txt
来源：http://hz.daria6918.cn/gtpljwwqco.html

[R49] awk 带条件
来源：http://hz.wangshuangyany.cn/gtbhxtpede.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ppjwa.cn/gtvtxwtejm.html

[R50] awk 求和
来源：http://hz.shangyingyoupin.top/gtdmdfvvfy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sysykeji.top/gtbbsxukhf.html

[R51] 排序去重取前几
来源：http://hz.jinqigufen.top/gtjawspafm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cheryme.top/gtpeelsraa.html

[R52] 统计行数
来源：http://hz.fengsongda.top/gtprrkkpcn.html

wc -l a.txt
来源：http://hz.yanxiufei.cn/gtoyrgaugl.html

[R53] 查看文件头与实时尾
来源：http://hz.ppjwa.cn/gtsmhekrgp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pycfn.com/gtxvniktit.html

[R54] 比较两个文件
来源：http://hz.kuanghao11.cn/gtvbzmvcfi.html

diff a.txt b.txt
来源：http://hz.yj20258.top/gtlcpmwixz.html

[R55] 压缩与解压
来源：http://hz.birdmap.top/gtdjnbfzbu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj202588.top/gtlhwmxkyb.html

[R56] 远程拷贝
来源：http://hz.guowangkeji.top/gtgnbiourf.html

scp file user@host:/path/
来源：http://hz.jiagoushi.top/gtrzpshutg.html

[R57] 远程执行命令
来源：http://hz.c1oappe.top/gtjtkghrsb.html

ssh user@host 'uptime'
来源：http://hz.quarkkingdee.top/gtotqfheqx.html

[R58] 下载文件
来源：http://hz.chenjidiqi.icu/gttebsrqla.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jqgfzy.top/gtjkyvwswb.html

[R59] 发 POST JSON
来源：http://hz.jinghuilouyu.cn/gtsicfnyxn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cashguo.top/gtjhcvcgnm.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtbixumupg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhongyouzk.top/gtzxeiinnz.html

[R61] 磁盘占用
来源：http://hz.daria6918.cn/gtxlnjnjvr.html

df -h;  du -sh *
来源：http://hz.birdmap.top/gtdpdqpusc.html

[R62] 找最占空间的文件
来源：http://hz.zycfv.cn/gtcjhozfoc.html

du -ah . | sort -rh | head -10
来源：http://hz.zycfv.cn/gtpxzinzal.html

[R63] 内存与进程
来源：http://hz.redwolf501.top/gtowhmngxs.html

free -h;  ps aux | grep nginx
来源：http://hz.cqqwz.cn/gtvsvehylq.html

[R64] 结束进程
来源：http://hz.jiagoushi.top/gtxugmzdrk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zdqjudy.top/gtkqkmmcce.html

[R65] 查看端口占用
来源：http://hz.0kj1m.cn/gtmaljisvg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xziqi.cn/gtmvcnfhgm.html

[R66] 定时任务
来源：http://hz.yangfankeji.com/gtbyzfndfr.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gtwbgcwxti.html

[R67] 生成随机十六进制串
来源：http://hz.daxiang520.top/gtrpxrdxav.html

openssl rand -hex 16
来源：http://hz.yj20258888.top/gtijbaaycd.html

[R68] 计算文件校验值
来源：http://hz.vqdsnc.cn/gtdgfynzep.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jianghu66.top/gtpqcmnjbk.html

[R69] 生成随机密码
来源：http://hz.zhijiandao.cn/gtpotzpqhs.html

head -c 16 /dev/urandom | base64
来源：http://hz.hfpthk.cn/gtkkqtlhce.html

[R70] 时间戳与互转
来源：http://hz.sweek.top/gtsqacpzvb.html

date +%s;  date -d @1700000000
来源：http://hz.zhengqikj.top/gtnkegdlxk.html

[R71] 日期格式化
来源：http://hz.nwbrower.top/gtsksewqrm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jianghu66.top/gtqmhlaefl.html

[R72] 等待端口就绪
来源：http://hz.316326.xyz/gtrowalcwk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtqopofanb.html

[R73] 分割大日志
来源：http://hz.dianchejie.cn/gtvcbwdgof.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtxrdpdagu.html

[R74] 批量重命名
来源：http://hz.kuanghao11.cn/gtqilpholn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gtzxszzgzx.html

[R75] 导出环境变量
来源：http://hz.xziqi.cn/gtqgsczsvn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jianghu66.top/gtfwirqqbr.html

[R76] 使用临时文件
来源：http://hz.pengpengdd.cyou/gtvlygnxjv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtgbkjmqat.html

[R77] 读取用户输入
来源：http://hz.zhaomingkeji.xyz/gtavegawec.html

read -rp "请输入: " ans
来源：http://hz.hammf.cn/gthejjctap.html

[R78] 交互式菜单
来源：http://hz.yonumen.top/gtmetzukxh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yangfankeji.com/gtojwdrybv.html

[R79] 解析命令行选项
来源：http://hz.quarkkingdee.top/gtmvsgcmes.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yongpay.top/gtjsatdcgb.html

[R80] 查看脚本执行耗时
来源：http://hz.ydzc1.top/gtuvxgtpvr.html

time ./run.sh
来源：http://hz.jqgfzy.top/gtcmjyfrbk.html

================================================================================
来源：http://hz.gzhubu.top/gtycbmaoor.html

S. C / C++ 专题
来源：http://hz.yj20258.top/gtigmatdxh.html

================================================================================
来源：http://hz.yangfankeji.com/gtntaoffpz.html

[S01] C：Hello World
来源：http://hz.cdnleiting.top/gtuipfqrkv.html

#include <stdio.h>
来源：http://hz.cashguo.top/gtbzueaoln.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj20258.top/gtspkhsnzn.html

[S02] C：变量与格式化输出
来源：http://hz.fzhhl.top/gtnnoeisrf.html

int a = 10; printf("%d\n", a);
来源：http://hz.gzhubu.top/gtpfetdyga.html

[S03] C：读入整数
来源：http://hz.9152youxi.cn/gthuebbzob.html

int x; scanf("%d", &x);
来源：http://hz.nanxinkj.top/gtizjcphcl.html

[S04] C：字符串复制
来源：http://hz.52xcode.cn/gtgaoyxejg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.smart0.xyz/gtabvawsrt.html

[S05] C：字符串长度
来源：http://hz.hywenlv.cn/gtfhnfzumx.html

strlen(s)
来源：http://hz.birdmap.top/gthpavzrns.html

[S06] C：字符串比较
来源：http://hz.wangdashe.top/gtivwzxwgc.html

strcmp(a, b) == 0
来源：http://hz.birdmap.top/gtwlrrykin.html

[S07] C：数组遍历求和
来源：http://hz.ybcxt.top/gtluahmktf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yongpay.top/gttqbzcgav.html

[S08] C：动态内存分配与释放
来源：http://hz.jqgfzy.top/gtfsiyhgya.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.redwolf501.top/gtqiuumbeo.html

[S09] C：结构体定义与初始化
来源：http://hz.xinyue.icu/gtwdgzqukc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhiwuduotai.top/gtqauhbkwx.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gtnsqcatue.html

int *p = &a;  *p = 5;
来源：http://hz.52xcode.cn/gtcfzdbniv.html

[S11] C：逐行读文件
来源：http://hz.pengpengdd.cyou/gtbrrlkcjg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.andypj.xyz/gtjlgajoeq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cucudq.cn/gtzagjuslz.html

fclose(f);
来源：http://hz.aizwys.cn/gtuzezmwkk.html

[S12] C：写文件
来源：http://hz.svipenyu.cn/gtftpjtqxh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xuanzx.com/gtqatjwayj.html

[S13] C：宏定义
来源：http://hz.jqgfzy.top/gtfoxnzcqz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.svipenyu.cn/gtuhazwcej.html

[S14] C：枚举
来源：http://hz.hnxiangtu.top/gteohkorse.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gotoacloud.top/gtrpakqeux.html

[S15] C：类型转换
来源：http://hz.wangdashe.top/gttbvecgtb.html

(double) a / b
来源：http://hz.hnqzz.top/gtdjhupnxo.html

[S16] C：位操作置位
来源：http://hz.zhiwuduotai.top/gtkhmaqicg.html

x |= (1 << 3);
来源：http://hz.bjfxy.top/gtfqhbcowy.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtnzxpaqxc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fzhhl.top/gtitinvawm.html

[S18] C：命令行参数
来源：http://hz.jinyuanbaomall.cn/gtcfgpjrfl.html

int main(int argc, char **argv)
来源：http://hz.aibaodan.cn/gtwrypgdip.html

[S19] C：快速排序
来源：http://hz.zhijiandao.cn/gtrsnhlhyf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtfkhwijbf.html

[S20] C：二分查找
来源：http://hz.feifeiyinyue.top/gtvheysydx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtkzimclyc.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtoacnpmfh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cqqwz.cn/gtqabisyvk.html

[S22] C：字符串转数字
来源：http://hz.feifeiyinyue.top/gtwmybzcuu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.0kj1m.cn/gtokbcbshs.html

[S23] C：随机数
来源：http://hz.yueranfly.top/gthxdrdcwd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ivvv.top/gtszynwzva.html

[S24] C：获取本地时间
来源：http://hz.zdqjudy.top/gtuumikgwa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gtnagfmfvs.html

[S25] C：内存拷贝
来源：http://hz.zhixingplan.top/gtvshukpqv.html

memcpy(dst, src, n);
来源：http://hz.guowangkeji.top/gtzqtvlety.html

[S26] C：内存清零
来源：http://hz.sufxvd.cn/gtyhcjigsa.html

memset(a, 0, sizeof a);
来源：http://hz.xingfuxueyuan.xyz/gteyabspzx.html

[S27] C：定义常量
来源：http://hz.guowangkeji.top/gtzbppkxdy.html

const double PI = 3.14159;
来源：http://hz.nanxinkj.top/gtvxayzcrf.html

[S28] C：静态变量
来源：http://hz.zhixingplan.top/gtgpzjkpqz.html

static int counter = 0;
来源：http://hz.ivvv.top/gtdkehencq.html

[S29] C：变参函数
来源：http://hz.havefunace.top/gtjmimrriz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yongpay.top/gtiaprsupl.html

[S30] C：头文件保护
来源：http://hz.guannengcc.top/gtblecgjwp.html

#ifndef X_H
来源：http://hz.0kj1m.cn/gthawjiuyy.html

#define X_H
来源：http://hz.jinqigfzy.top/gtjobsifdk.html

#endif
来源：http://hz.sxryk.cn/gtpmggulbr.html

[S31] C++：Hello World
来源：http://hz.tanke756.top/gtejtpiies.html

#include <iostream>
来源：http://hz.mhx1999.top/gtlzkukcwr.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ybcxt.top/gtisgjnwpn.html

[S32] C++：字符串
来源：http://hz.pycfn.com/gtfutkapjh.html

std::string s = "hi";  s += "!";
来源：http://hz.xinyue.icu/gtbyevelyp.html

[S33] C++：vector 增删
来源：http://hz.xuetiantiany.cn/gtdjcligkv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gtixcootji.html

[S34] C++：遍历 vector
来源：http://hz.fengsongda.top/gtwewerdyh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shuidangran.top/gtqyhrwwer.html

[S35] C++：map
来源：http://hz.hywenlv.cn/gtqtxvpstn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.havefunace.top/gtftmfqtjp.html

[S36] C++：unordered_map
来源：http://hz.zdqjudy.top/gttefaydru.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtnxqvpbze.html

[S37] C++：set
来源：http://hz.pengpengdd.cyou/gtwrcmyywq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zdqjudy.top/gtltqonafg.html

[S38] C++：排序
来源：http://hz.jinghuilouyu.cn/gtapplgijv.html

std::sort(v.begin(), v.end());
来源：http://hz.hfpthk.cn/gtxqpxhrkk.html

[S39] C++：自定义比较器排序
来源：http://hz.ehwqpu.com/gtciklccwp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cdnleiting.top/gtntdqdfgk.html

[S40] C++：查找元素
来源：http://hz.zycfv.cn/gthfwijffn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ppjwa.cn/gtcccllcyk.html

[S41] C++：类与构造函数
来源：http://hz.zhixingplan.top/gtydywkwmz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xuetiantiany.cn/gtwjfuebtj.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gtztvaltcx.html

class B : public Base { public: void f() override {} };
来源：http://hz.xinyue.icu/gtzofnxscs.html

[S43] C++：智能指针
来源：http://hz.xziqi.cn/gtpyxfxayk.html

auto p = std::make_unique<int>(5);
来源：http://hz.52xcode.cn/gteefvmdky.html

[S44] C++：引用传参
来源：http://hz.zhongyouzk.top/gtunkcbbhs.html

void inc(int &x) { ++x; }
来源：http://hz.52xcode.cn/gtgrwppegk.html


<!-- 参考信息 -->