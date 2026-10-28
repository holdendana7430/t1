代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.andypj.xyz/gtaftqnyjt.html

[Q75] 日期格式化
来源：http://hz.pengpengdd.cyou/gtwdsdxric.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.meibo888.top/gttpfarmtn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.birdmap.top/gtajmcgkjp.html

[Q76] 按天统计
来源：http://hz.jinqigfzy.top/gtkcrsqisq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gaohongyu789.top/gtthrqxqkn.html

[Q77] 时间加减
来源：http://hz.chenjidiqi.icu/gtirhuryqv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.bjfxy.top/gtqusqrwri.html

[Q78] 当前时间
来源：http://hz.redwolf501.top/gtkufesyxw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.iojbl.cn/gtwuioclgv.html

[Q79] 字符串拼接
来源：http://hz.zdqjudy.top/gteaecnbrk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fengsongda.top/gtqhnmjnjo.html

[Q80] 字符串截取
来源：http://hz.snrcjt.cn/gtjjputlbo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj202588.top/gtallcyhqz.html

[Q81] 字符串替换
来源：http://hz.aizwys.cn/gtwoxbyazw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.dianchejie.cn/gtdnqzghxj.html

[Q82] 字符长度与字节长度
来源：http://hz.shuidangran.top/gtssslrviz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhengqikj.top/gtlclqhexv.html

[Q83] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtovbmosrx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtygmomvba.html

[Q84] 去除首尾空格
来源：http://hz.kuanghao11.cn/gtlwjxuvpv.html

SELECT TRIM(name) FROM users;
来源：http://hz.feifeiyinyue.top/gtffyuqzrt.html

[Q85] 数值取整
来源：http://hz.jyoumei.cn/gtqkfbdmat.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.bjfxy.top/gtzkgcfuxt.html

[Q86] 读取 JSON 字段
来源：http://hz.yuanzhike.top/gtjjjbptgz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xziqi.cn/gtmzdbubct.html

[Q87] JSON 字段做条件
来源：http://hz.cucudq.cn/gtigmzymwe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.sufxvd.cn/gtrkeiknld.html

[Q88] 行转列（条件聚合）
来源：http://hz.yj20258888.top/gtuuapvbor.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yuxming.cn/gtdqklpjog.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sweek.top/gtsyibcuda.html

[Q89] 判断表是否存在
来源：http://hz.zdqjudy.top/gtketzzebq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ybcxt.top/gtzyuarqkb.html

[Q90] 生成序号列
来源：http://hz.yj20258.top/gtpmqdkiqg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.daxiang520.top/gtaxipfvqj.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwpojahnj.html

R. Bash 专题
来源：http://hz.jinqigufen.top/gtbadxqmju.html

================================================================================
来源：http://hz.sxryk.cn/gtlftlcrcu.html

[R01] shebang 与严格模式
来源：http://hz.ywan-chungtsiang.top/gtiwnwcjhz.html

#!/usr/bin/env bash
来源：http://hz.andypj.xyz/gtxtucwlum.html

set -euo pipefail
来源：http://hz.cheryme.top/gtqeswzqhc.html

[R02] 变量赋值与使用
来源：http://hz.xuanzx.com/gtjxkxpfkz.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtnfdybpwq.html

[R03] 只读变量
来源：http://hz.nanxinkj.top/gtpfvcxkns.html

readonly PI=3.14
来源：http://hz.cucudq.cn/gtjubiidhf.html

[R04] 位置参数
来源：http://hz.zhoulong.xyz/gtxztcwlhe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.snrcjt.cn/gtawgcqnsg.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtqitujzdn.html

name="${1:-default}"
来源：http://hz.fengsongda.top/gtnuygaciz.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtzqwmzppo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.pengpengdd.cyou/gtebvzroda.html

[R07] if 判断文件
来源：http://hz.shzxlz.cn/gtiomsdiqp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cqqwz.cn/gtsegaxirn.html

[R08] 数值比较
来源：http://hz.tian-w.cn/gtwhjruoin.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ehwqpu.com/gthyqtntic.html

[R09] 字符串比较
来源：http://hz.ppjwa.cn/gtsqhobhul.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tianlin.xyz/gtdsfepyza.html

[R10] 正则匹配
来源：http://hz.yueranfly.top/gtzajvbpek.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dashuyun.cn/gtyocdrmdf.html

[R11] case 多分支
来源：http://hz.pengpengdd.cyou/gtvgbljkpj.html

case "$1" in
来源：http://hz.zhiwuduotai.top/gtorjshnpe.html

start) echo "启动" ;;
来源：http://hz.nanxuanxn.top/gttnindtzo.html

stop)  echo "停止" ;;
来源：http://hz.tian-w.cn/gteyefxkly.html

*)     echo "未知命令" ;;
来源：http://hz.hnxiangtu.top/gtgdnmucwe.html

esac
来源：http://hz.sxryk.cn/gtikcdarvt.html

[R12] for 遍历文件
来源：http://hz.xingfuxueyuan.xyz/gthbizlagw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cdnleiting.top/gtanqlcfgl.html

[R13] for 计数循环
来源：http://hz.kuanghao11.cn/gtisehwayx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aizwys.cn/gtbiwwhyuc.html

[R14] C 风格 for
来源：http://hz.daria6918.cn/gtiupyfuqv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhoulong.xyz/gtptotzuud.html

[R15] while 逐行读文件
来源：http://hz.zdqjudy.top/gtljrbdxiu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xuanzx.com/gtoodiismh.html

[R16] until 等待条件
来源：http://hz.guannengcc.top/gtqmgfysqy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.snrcjt.cn/gtcfpqhbiw.html

[R17] 数组定义与取值
来源：http://hz.jianghu66.top/gtxlbsbyug.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cqqwz.cn/gtrryjpdpu.html

[R18] 遍历数组
来源：http://hz.cqqwz.cn/gtrkbzvmks.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.feifeiyinyue.top/gtmxzvksaj.html

[R19] 数组长度
来源：http://hz.chenjidiqi.icu/gtmsdluwev.html

echo "${#arr[@]}"
来源：http://hz.tian-w.cn/gtjqmytxln.html

[R20] 关联数组（字典）
来源：http://hz.bjfxy.top/gtlpnhjxai.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtwyddficl.html

[R21] 字符串长度
来源：http://hz.yueranfly.top/gtsnxtkusi.html

echo "${#s}"
来源：http://hz.yj202588.top/gtyarxmmip.html

[R22] 截取子串
来源：http://hz.zhijiandao.cn/gtazrmwrlb.html

echo "${s:0:5}"
来源：http://hz.jinqigufen.top/gtozputeta.html

[R23] 字符串替换
来源：http://hz.jqgufenzy.top/gtqkixghjn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.guowangkeji.top/gtodvrjecq.html

[R24] 大小写转换
来源：http://hz.yj20258888.top/gtvhlusyft.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.316326.xyz/gtddqldwcb.html

[R25] 去后缀 / 去前缀
来源：http://hz.shangyingyoupin.top/gtqwrntewp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenzaomai.com/gtozbbrbcd.html

[R26] 命令替换
来源：http://hz.guannengcc.top/gtqxskibpw.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gttswwbaql.html

[R27] 算术展开
来源：http://hz.smart0.xyz/gtglxwubmq.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gtwddjdofx.html

[R28] 浮点运算
来源：http://hz.jinqigufen.top/gtrqojcueu.html

echo "scale=2; 10/3" | bc
来源：http://hz.316326.xyz/gthwalxuid.html

[R29] 定义函数
来源：http://hz.chenzaomai.com/gtczdwwqos.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hfpthk.cn/gtxokhituo.html

[R30] 函数返回状态码
来源：http://hz.quarkkingdee.top/gtartdsbgf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gotoacloud.top/gtjynbraar.html

[R31] 局部变量
来源：http://hz.xziqi.cn/gtisccebif.html

f() { local x=1; echo "$x"; }
来源：http://hz.jinqigufen.top/gtivmydcur.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gtakwdqmpv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.svipenyu.cn/gtextiobux.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtlywjqxeu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuanzx.com/gtexusavhk.html

[R34] 退出时清理
来源：http://hz.pycfn.com/gttmsbclbq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.vqdsnc.cn/gtrwidyaht.html

[R35] 后台执行并等待
来源：http://hz.meibo888.top/gtzmqtgetv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhongyouzk.top/gtlcexbjkm.html

[R36] 并发执行多个任务
来源：http://hz.ywan-chungtsiang.top/gtcxnzlnmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nwbrower.top/gtpmodtczi.html

[R37] 把输出赋给变量
来源：http://hz.cucudq.cn/gtqmamrkge.html

files=$(ls -1)
来源：http://hz.sysykeji.top/gtkpzsmcgs.html

[R38] 管道串联
来源：http://hz.hammf.cn/gtpeuhizng.html

cat a.txt | grep -i error | wc -l
来源：http://hz.dianchejie.cn/gtroscrhtt.html

[R39] 重定向标准输出与错误
来源：http://hz.yueranfly.top/gtkbjgscri.html

cmd > out.log 2>&1
来源：http://hz.shzxlz.cn/gtkbildkte.html

[R40] 追加写日志
来源：http://hz.haohaochexian.top/gtfpkmjbyi.html

echo "log" >> out.log
来源：http://hz.guannengcc.top/gtjfeysnww.html

[R41] 丢弃输出
来源：http://hz.sufxvd.cn/gtsnjspuun.html

cmd >/dev/null 2>&1
来源：http://hz.yuxming.cn/gtmaltohoc.html

[R42] 输入重定向
来源：http://hz.xingfuxueyuan.xyz/gtzpbvcroe.html

wc -l < a.txt
来源：http://hz.wangdashe.top/gtimwtbhfv.html

[R43] 按名字查找文件
来源：http://hz.tianlin.xyz/gtwkhbkwiq.html

find . -name "*.log" -type f
来源：http://hz.jyoumei.cn/gtzoxocznr.html

[R44] 按修改时间查找
来源：http://hz.gaohongyu789.top/gtqkgqubyz.html

find . -mtime -7 -type f
来源：http://hz.xingfuxueyuan.xyz/gtkxuotqts.html

[R45] 批量删除
来源：http://hz.xuetiantiany.cn/gtodfqfrnv.html

find . -name "*.tmp" -delete
来源：http://hz.yuxming.cn/gtwyqdizug.html

[R46] 递归替换文件内容
来源：http://hz.zhongyouzk.top/gtijsqlzyi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.birdmap.top/gtydtvcrru.html

[R47] sed 单行替换
来源：http://hz.ybcxt.top/gtrzxfecbl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydzc1.top/gtxaqsmlsi.html

[R48] awk 取指定列
来源：http://hz.ybcxt.top/gtlfxexcbr.html

awk '{print $1, $3}' a.txt
来源：http://hz.snrcjt.cn/gtyjwcxigj.html

[R49] awk 带条件
来源：http://hz.vqdsnc.cn/gttmvumlqz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.bjfxy.top/gtnzcfegki.html

[R50] awk 求和
来源：http://hz.gogol.net.cn/gtzviohxwn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.feifeiyinyue.top/gtmprmqcve.html

[R51] 排序去重取前几
来源：http://hz.zhengqikj.top/gtamsbhjwe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hammf.cn/gtgeekthvx.html

[R52] 统计行数
来源：http://hz.iojbl.cn/gtusdejpzq.html

wc -l a.txt
来源：http://hz.yuxming.cn/gtttduhbvb.html

[R53] 查看文件头与实时尾
来源：http://hz.wangshuangyany.cn/gtuhdgujdr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenzaomai.com/gtujkeslrw.html

[R54] 比较两个文件
来源：http://hz.sweek.top/gtuewailhf.html

diff a.txt b.txt
来源：http://hz.smart0.xyz/gtiwtqzfhk.html

[R55] 压缩与解压
来源：http://hz.xuanzx.com/gtopwfwoll.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guannengcc.top/gtbrszfhzl.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gtqgdgtfts.html

scp file user@host:/path/
来源：http://hz.jqgfzy.top/gtrvkbrplu.html

[R57] 远程执行命令
来源：http://hz.tianlin.xyz/gtgujdtblg.html

ssh user@host 'uptime'
来源：http://hz.xuanzx.com/gtpdcolvyv.html

[R58] 下载文件
来源：http://hz.gotoacloud.top/gtqtmzmxrk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yuanzhike.top/gthchnbuep.html

[R59] 发 POST JSON
来源：http://hz.fengsongda.top/gtblklilwb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jqgfzy.top/gtrwwyqibm.html

[R60] 只看 HTTP 状态码
来源：http://hz.dashuyun.cn/gtabyczwlw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigfzy.top/gtjdrxsfdv.html

[R61] 磁盘占用
来源：http://hz.daxiang520.top/gtoxnvlzfh.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gthwmqncna.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtlnfvgvre.html

du -ah . | sort -rh | head -10
来源：http://hz.jyoumei.cn/gtmtxzpiff.html

[R63] 内存与进程
来源：http://hz.bjfxy.top/gtcpvkcpwv.html

free -h;  ps aux | grep nginx
来源：http://hz.gogol.net.cn/gtcmdcpoam.html

[R64] 结束进程
来源：http://hz.yj20258.top/gthlvbcnsh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yonumen.top/gtuiqurrhf.html

[R65] 查看端口占用
来源：http://hz.yonumen.top/gthnldiwjo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hywenlv.cn/gthlzsbsag.html

[R66] 定时任务
来源：http://hz.wangdashe.top/gtkhibnzet.html

crontab -e;  crontab -l
来源：http://hz.c1oappe.top/gtydowmamo.html

[R67] 生成随机十六进制串
来源：http://hz.hysaishi.cn/gterpbmmey.html

openssl rand -hex 16
来源：http://hz.daxiang520.top/gticivaeli.html

[R68] 计算文件校验值
来源：http://hz.shangyingyoupin.top/gtmuqcvhje.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ppjwa.cn/gtxjcprbde.html

[R69] 生成随机密码
来源：http://hz.cqqwz.cn/gtetqygihj.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinqigfzy.top/gtmhnbzhyg.html

[R70] 时间戳与互转
来源：http://hz.jyoumei.cn/gtexgquckr.html

date +%s;  date -d @1700000000
来源：http://hz.snrcjt.cn/gtrzrwblsr.html

[R71] 日期格式化
来源：http://hz.jianghu66.top/gtdvcedssz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nanxuanxn.top/gtmadgkjpe.html

[R72] 等待端口就绪
来源：http://hz.hongshengwenyu.top/gtjgaxxltg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jianghu66.top/gtomelaksz.html

[R73] 分割大日志
来源：http://hz.ppjwa.cn/gtidnppdlb.html

split -l 1000 big.log part_
来源：http://hz.hysaishi.cn/gtrnlepsmy.html

[R74] 批量重命名
来源：http://hz.0kj1m.cn/gtfawgvzxq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hfpthk.cn/gtnurpxfti.html

[R75] 导出环境变量
来源：http://hz.shanyushiyangtech.top/gtiurrogcp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigfzy.top/gtddvuedty.html

[R76] 使用临时文件
来源：http://hz.gzhubu.top/gtcvjvwjhg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gtqylhsqtg.html

[R77] 读取用户输入
来源：http://hz.xinyue.icu/gtdptkvmjm.html

read -rp "请输入: " ans
来源：http://hz.dashuyun.cn/gtcsanqrqo.html

[R78] 交互式菜单
来源：http://hz.guannengcc.top/gtfzxfdxkc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yangfankeji.com/gtqayaqacn.html

[R79] 解析命令行选项
来源：http://hz.pengpengdd.cyou/gtkaeegvho.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.andypj.xyz/gtrodkotif.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gtmqgbesgi.html

time ./run.sh
来源：http://hz.guannengcc.top/gtryvvslyf.html

================================================================================
来源：http://hz.zhengqikj.top/gtqpqotvqb.html

S. C / C++ 专题
来源：http://hz.jyoumei.cn/gtvoaeqlxn.html

================================================================================
来源：http://hz.cashguo.top/gtexmfxzlx.html

[S01] C：Hello World
来源：http://hz.hammf.cn/gtcisycabv.html

#include <stdio.h>
来源：http://hz.zhoulong.xyz/gtamzwvnxk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gotoacloud.top/gtcwlnzbeb.html

[S02] C：变量与格式化输出
来源：http://hz.xuetiantiany.cn/gtfltonhly.html

int a = 10; printf("%d\n", a);
来源：http://hz.sxryk.cn/gtgfkhotsq.html

[S03] C：读入整数
来源：http://hz.zhiwuduotai.top/gtizhtuoyr.html

int x; scanf("%d", &x);
来源：http://hz.andypj.xyz/gtdkemsjqm.html

[S04] C：字符串复制
来源：http://hz.c1oappe.top/gtvsfbdjkd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gteeuhuxqn.html

[S05] C：字符串长度
来源：http://hz.xylfe.cn/gthkloepxn.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gtfpiuyklm.html

[S06] C：字符串比较
来源：http://hz.sufxvd.cn/gtaqxlpgcv.html

strcmp(a, b) == 0
来源：http://hz.yvedp.cn/gtpkjnifzu.html

[S07] C：数组遍历求和
来源：http://hz.ydzc1.top/gtfkkecaps.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shuidangran.top/gtlqhhsdra.html

[S08] C：动态内存分配与释放
来源：http://hz.yueranfly.top/gtoodfdvif.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.316326.xyz/gtgnstolzt.html

[S09] C：结构体定义与初始化
来源：http://hz.chenjidiqi.icu/gthvujmmwi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.meibo888.top/gtnivoinip.html

[S10] C：指针与解引用
来源：http://hz.yuanzhike.top/gtmxccvyja.html

int *p = &a;  *p = 5;
来源：http://hz.ehwqpu.com/gtxahdojgd.html

[S11] C：逐行读文件
来源：http://hz.sysykeji.top/gtnhivpeio.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dashuyun.cn/gtomgcrajq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yonumen.top/gtxezoscid.html

fclose(f);
来源：http://hz.zhijiandao.cn/gtgoticjyq.html

[S12] C：写文件
来源：http://hz.smart0.xyz/gtfpteamkj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sufxvd.cn/gtiwiaypkp.html

[S13] C：宏定义
来源：http://hz.gzhubu.top/gtepuwqvwz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sxryk.cn/gteclmiruh.html

[S14] C：枚举
来源：http://hz.pengpengdd.cyou/gtexfzbraw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tianlin.xyz/gtaydrhfbw.html

[S15] C：类型转换
来源：http://hz.jyoumei.cn/gtfzzqcydo.html

(double) a / b
来源：http://hz.yuxming.cn/gtcxewjolq.html

[S16] C：位操作置位
来源：http://hz.yonumen.top/gtetqdfhtt.html

x |= (1 << 3);
来源：http://hz.havefunace.top/gtycuumorb.html

[S17] C：安全拼接字符串
来源：http://hz.nanxuanxn.top/gtqawgnvbc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cqqwz.cn/gteetgzydt.html

[S18] C：命令行参数
来源：http://hz.zycfv.cn/gttzymfifg.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gtkawazqsr.html

[S19] C：快速排序
来源：http://hz.jqgufenzy.top/gtdfozeqyl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.smart0.xyz/gthsbzxapl.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtaistnked.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtmwabnwol.html

[S21] C：字符类别判断
来源：http://hz.zycfv.cn/gthkmhdmkd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gtynczrfmo.html

[S22] C：字符串转数字
来源：http://hz.yongpay.top/gtpzhjiuqq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhijiandao.cn/gtvnurtmvc.html

[S23] C：随机数
来源：http://hz.sysykeji.top/gtcxmhqvlv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gaohongyu789.top/gthvupcizb.html

[S24] C：获取本地时间
来源：http://hz.kuanghao11.cn/gtmaajyffh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fengsongda.top/gtpamgunym.html

[S25] C：内存拷贝
来源：http://hz.9152youxi.cn/gtblaoqwgt.html

memcpy(dst, src, n);
来源：http://hz.shanyushiyangkeji.top/gtskvwypik.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gtpeuqnbqv.html

memset(a, 0, sizeof a);
来源：http://hz.daria6918.cn/gtyhwfasgm.html

[S27] C：定义常量
来源：http://hz.dianchejie.cn/gtgolngufu.html

const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtghascrle.html

[S28] C：静态变量
来源：http://hz.snrcjt.cn/gtcpqygnbo.html

static int counter = 0;
来源：http://hz.yongpay.top/gtlqxcbsfr.html

[S29] C：变参函数
来源：http://hz.jlsjyb.cn/gtnrfrptku.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtmdbleims.html

[S30] C：头文件保护
来源：http://hz.hnqzz.top/gtovsewvxe.html

#ifndef X_H
来源：http://hz.bjfxy.top/gtouzotvbl.html

#define X_H
来源：http://hz.iojbl.cn/gtmlfcuyfu.html

#endif
来源：http://hz.guannengcc.top/gtgtytvicf.html

[S31] C++：Hello World
来源：http://hz.bjfxy.top/gtikyraufv.html

#include <iostream>
来源：http://hz.jinqigufen.top/gtxcuibncy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hnxiangtu.top/gtglhwkllj.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gtywxfdsvb.html

std::string s = "hi";  s += "!";
来源：http://hz.jyoumei.cn/gtzrtaysqo.html

[S33] C++：vector 增删
来源：http://hz.dianchejie.cn/gtnmsjilej.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtsadwzuir.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtzzcinedz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.quarkkingdee.top/gtxwkvgjmg.html

[S35] C++：map
来源：http://hz.chenzaomai.com/gtynbhnruh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtuuhvcxxm.html

[S36] C++：unordered_map
来源：http://hz.daxiang520.top/gtsjcqiseb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtvidbjfmy.html

[S37] C++：set
来源：http://hz.chenlongwang.top/gtncpvtpdq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenlongwang.top/gtdlsdbtgo.html

[S38] C++：排序
来源：http://hz.jqgufenzy.top/gtutuczpsz.html

std::sort(v.begin(), v.end());
来源：http://hz.hongshengwenyu.top/gtaloiwsop.html

[S39] C++：自定义比较器排序
来源：http://hz.ehwqpu.com/gtogyntoyp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pycfn.com/gtoqbfhbit.html

[S40] C++：查找元素
来源：http://hz.hnqzz.top/gtbhkwwogg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.pycfn.com/gtgjcjhthv.html

[S41] C++：类与构造函数
来源：http://hz.yj20258888.top/gtdxxvutlu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yangfankeji.com/gtnqtwkwxn.html

[S42] C++：继承与虚函数
来源：http://hz.chenjidiqi.icu/gtzxggogsg.html

class B : public Base { public: void f() override {} };
来源：http://hz.jyoumei.cn/gthswyjmcz.html

[S43] C++：智能指针
来源：http://hz.jlsjyb.cn/gtmhwalnik.html

auto p = std::make_unique<int>(5);
来源：http://hz.xuanzx.com/gtydsjeqvg.html

[S44] C++：引用传参
来源：http://hz.havefunace.top/gtphwzqvah.html

void inc(int &x) { ++x; }
来源：http://hz.sxryk.cn/gtqfkmgsas.html


<!-- 参考信息 -->