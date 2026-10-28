代发 wailian999

[Q67] 设置隔离级别
来源：http://hz.aibaodan.cn/gtqlwyhljl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cqqwz.cn/gtkmesqgey.html

[Q68] 保存点
来源：http://hz.xinyue.icu/gtpinvmabi.html

SAVEPOINT sp1;
来源：http://hz.cheryme.top/gtarunotpt.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtsxwcsyhk.html

[Q69] 查看执行计划
来源：http://hz.yangfankeji.com/gtfcmictfu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.quarkkingdee.top/gtbpxkhbko.html

[Q70] 更新统计信息
来源：http://hz.daria6918.cn/gtprlufsue.html

ANALYZE TABLE users;
来源：http://hz.iojbl.cn/gtcercxfzh.html

[Q71] 查看建表语句
来源：http://hz.guowangkeji.top/gtcnypcnzm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.redwolf501.top/gtfugtolae.html

[Q72] 查看索引
来源：http://hz.nwbrower.top/gtlshrkuvj.html

SHOW INDEX FROM users;
来源：http://hz.birdmap.top/gtuwawinou.html

[Q73] 查看表状态
来源：http://hz.dianchejie.cn/gtxhqudkds.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.iojbl.cn/gtdivfrpwu.html

[Q74] 强制使用索引
来源：http://hz.hnqzz.top/gtpqeuuvzt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.mhx1999.top/gtrfkxydjg.html

[Q75] 日期格式化
来源：http://hz.zdqjudy.top/gtpjehtces.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenzaomai.com/gtzpzpdoiv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xinyue.icu/gthfqeqobx.html

[Q76] 按天统计
来源：http://hz.sufxvd.cn/gtsrimszen.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.pengpengdd.cyou/gtbvvmpoxy.html

[Q77] 时间加减
来源：http://hz.gaohongyu789.top/gtbfrvwztq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zycfv.cn/gtjlojvivk.html

[Q78] 当前时间
来源：http://hz.vqdsnc.cn/gtuhvfxajq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258888.top/gtcvlgcxlr.html

[Q79] 字符串拼接
来源：http://hz.dashuyun.cn/gthlqpmhcl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigfzy.top/gtxawtjkig.html

[Q80] 字符串截取
来源：http://hz.zhongyouzk.top/gtdfmmotjg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj202588.top/gtarerpjut.html

[Q81] 字符串替换
来源：http://hz.nanxinkj.top/gtraaitwnk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tanke756.top/gtlyykhhyo.html

[Q82] 字符长度与字节长度
来源：http://hz.wangshuangyany.cn/gthyrqgqnn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jqgfzy.top/gtfygdcrbo.html

[Q83] 大小写转换
来源：http://hz.haohaochexian.top/gtafbleari.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.cucudq.cn/gtspcszqsk.html

[Q84] 去除首尾空格
来源：http://hz.pycfn.com/gtnaalqeew.html

SELECT TRIM(name) FROM users;
来源：http://hz.ivvv.top/gtjnnjfxmy.html

[Q85] 数值取整
来源：http://hz.yonumen.top/gtfamdubnd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nanxuanxn.top/gtddphcukv.html

[Q86] 读取 JSON 字段
来源：http://hz.jianghu66.top/gtoumclchc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinghuilouyu.cn/gtdevzvvfd.html

[Q87] JSON 字段做条件
来源：http://hz.kuanghao11.cn/gttiqfzqnc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shuidangran.top/gtnwbobigs.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenzaomai.com/gtwuouhjfj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tian-w.cn/gtyzzvzkkz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.shanyushiyangkeji.top/gtkulzdzlx.html

[Q89] 判断表是否存在
来源：http://hz.daria6918.cn/gtqiaepslu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xinyue.icu/gtxuyxntbp.html

[Q90] 生成序号列
来源：http://hz.316326.xyz/gttkornuad.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xinyue.icu/gtjtvxzodq.html

================================================================================
来源：http://hz.pycfn.com/gtvbtfsgou.html

R. Bash 专题
来源：http://hz.guowangkeji.top/gtrhosxocq.html

================================================================================
来源：http://hz.fzhhl.top/gtzwixnupy.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangkeji.top/gttwdcqvsl.html

#!/usr/bin/env bash
来源：http://hz.zdqjudy.top/gtogcdvabu.html

set -euo pipefail
来源：http://hz.iojbl.cn/gtndpjkrxa.html

[R02] 变量赋值与使用
来源：http://hz.iojbl.cn/gtifjianvw.html

name="Tom"; echo "$name"
来源：http://hz.wangdashe.top/gtmbnljcmc.html

[R03] 只读变量
来源：http://hz.jianghu66.top/gtsrqlxhzk.html

readonly PI=3.14
来源：http://hz.jyoumei.cn/gtchckmqac.html

[R04] 位置参数
来源：http://hz.hnqzz.top/gtkobefjra.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sxryk.cn/gtigqjclix.html

[R05] 参数默认值
来源：http://hz.tian-w.cn/gtngrylphf.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtqgdocklp.html

[R06] 判断命令是否存在
来源：http://hz.redwolf501.top/gtsrttifod.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jyoumei.cn/gttpqhrbcc.html

[R07] if 判断文件
来源：http://hz.0kj1m.cn/gtzglbxvns.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.meibo888.top/gtysbiaawt.html

[R08] 数值比较
来源：http://hz.hfpthk.cn/gtqvsfaaxd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yonumen.top/gtkxzkcfzd.html

[R09] 字符串比较
来源：http://hz.xinyue.icu/gtxtajwupb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hfpthk.cn/gtsutwppxh.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtouioxlgk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yonumen.top/gtmqjmectq.html

[R11] case 多分支
来源：http://hz.yangfankeji.com/gtezzcrhnl.html

case "$1" in
来源：http://hz.hysaishi.cn/gtthkmgims.html

start) echo "启动" ;;
来源：http://hz.fzhhl.top/gtykanomzz.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gtgtjlrdlp.html

*)     echo "未知命令" ;;
来源：http://hz.yj20258888.top/gtranjnzdg.html

esac
来源：http://hz.jinqigufen.top/gtktudyiqu.html

[R12] for 遍历文件
来源：http://hz.hongshengwenyu.top/gtvxvvgpzi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sweek.top/gtbnbcrqyf.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gtrunhtphr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ywan-chungtsiang.top/gtqhypncvp.html

[R14] C 风格 for
来源：http://hz.ydzc1.top/gtzxxbrplw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtppabuozf.html

[R15] while 逐行读文件
来源：http://hz.ppjwa.cn/gtfhnqoait.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.0kj1m.cn/gtthctvcug.html

[R16] until 等待条件
来源：http://hz.snrcjt.cn/gtdkehxxoj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hfpthk.cn/gtvopcyiwn.html

[R17] 数组定义与取值
来源：http://hz.zycfv.cn/gtedbsvxyo.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hfpthk.cn/gteaskbkxk.html

[R18] 遍历数组
来源：http://hz.nwbrower.top/gtbvwsqsjc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fzhhl.top/gtonqdscst.html

[R19] 数组长度
来源：http://hz.c1oappe.top/gtojuqmels.html

echo "${#arr[@]}"
来源：http://hz.chenlongwang.top/gtswwvvtbv.html

[R20] 关联数组（字典）
来源：http://hz.zhaomingkeji.xyz/gtfoxeemgs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gthnvajufj.html

[R21] 字符串长度
来源：http://hz.yj20258.top/gtrxrqxwjb.html

echo "${#s}"
来源：http://hz.sufxvd.cn/gtfwnbojei.html

[R22] 截取子串
来源：http://hz.cheryme.top/gtshtokemy.html

echo "${s:0:5}"
来源：http://hz.cqqwz.cn/gtnocrubyy.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtnbobkndq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gtpxuhslhe.html

[R24] 大小写转换
来源：http://hz.zhongyouzk.top/gtrlusgyak.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.andypj.xyz/gtqxzhikbv.html

[R25] 去后缀 / 去前缀
来源：http://hz.aizwys.cn/gtocjcdwkr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnqzz.top/gtozvsupup.html

[R26] 命令替换
来源：http://hz.mhx1999.top/gteiucrhla.html

now=$(date +%F); echo "$now"
来源：http://hz.chenzaomai.com/gtycyiqmwf.html

[R27] 算术展开
来源：http://hz.xuetiantiany.cn/gtkxaqovcj.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gttkcqxpiq.html

[R28] 浮点运算
来源：http://hz.xuetiantiany.cn/gtaxhwoqcv.html

echo "scale=2; 10/3" | bc
来源：http://hz.hammf.cn/gtaowvbzqt.html

[R29] 定义函数
来源：http://hz.jiagoushi.top/gtvlwgwpbw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.pengpengdd.cyou/gtmgkaseol.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtnolqfwsi.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cucudq.cn/gtfhhnbwmb.html

[R31] 局部变量
来源：http://hz.mhx1999.top/gtymwbdebj.html

f() { local x=1; echo "$x"; }
来源：http://hz.ydzc1.top/gtlvjomrlk.html

[R32] 参数个数校验
来源：http://hz.cashguo.top/gtwcrdsmob.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zdqjudy.top/gtldgryjoz.html

[R33] 捕获错误并提示行号
来源：http://hz.ydzc1.top/gthntildlk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtwvqkrybj.html

[R34] 退出时清理
来源：http://hz.zhijiandao.cn/gtzjjtfdzs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daxiang520.top/gtdoxnnlau.html

[R35] 后台执行并等待
来源：http://hz.jinyuanbaomall.cn/gtlplwaovj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shzxlz.cn/gtymeakifb.html

[R36] 并发执行多个任务
来源：http://hz.ivvv.top/gtgrmdboeh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.meibo888.top/gteupiteun.html

[R37] 把输出赋给变量
来源：http://hz.hongshengwenyu.top/gtxgtroraz.html

files=$(ls -1)
来源：http://hz.havefunace.top/gtpgrwuwyf.html

[R38] 管道串联
来源：http://hz.jinyuanbaomall.cn/gtrpjvorzp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.iojbl.cn/gtuoqclzui.html

[R39] 重定向标准输出与错误
来源：http://hz.cqqwz.cn/gtlzimokry.html

cmd > out.log 2>&1
来源：http://hz.yueranfly.top/gtgaviwqke.html

[R40] 追加写日志
来源：http://hz.fengsongda.top/gtokdeiuau.html

echo "log" >> out.log
来源：http://hz.yueranfly.top/gtphllqbii.html

[R41] 丢弃输出
来源：http://hz.sxryk.cn/gtwcrmsadp.html

cmd >/dev/null 2>&1
来源：http://hz.zdqjudy.top/gtzrzbsdke.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtqwtxxbrv.html

wc -l < a.txt
来源：http://hz.xinyue.icu/gtchoxhcjw.html

[R43] 按名字查找文件
来源：http://hz.ybcxt.top/gtigrcgppz.html

find . -name "*.log" -type f
来源：http://hz.redwolf501.top/gtfysuxmnu.html

[R44] 按修改时间查找
来源：http://hz.svipenyu.cn/gtfbhsjlns.html

find . -mtime -7 -type f
来源：http://hz.aizwys.cn/gtsrjzxbvc.html

[R45] 批量删除
来源：http://hz.ywan-chungtsiang.top/gtdmtnvjse.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtpnabsffq.html

[R46] 递归替换文件内容
来源：http://hz.andypj.xyz/gtgtxwutdg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.havefunace.top/gtretoonyg.html

[R47] sed 单行替换
来源：http://hz.tanke756.top/gtkbliiyas.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.havefunace.top/gtoksfceny.html

[R48] awk 取指定列
来源：http://hz.ivvv.top/gtmybhzjoy.html

awk '{print $1, $3}' a.txt
来源：http://hz.fzhhl.top/gtnibkqaye.html

[R49] awk 带条件
来源：http://hz.tianlin.xyz/gtnvjrqiib.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hywenlv.cn/gtfystlirs.html

[R50] awk 求和
来源：http://hz.jinqigfzy.top/gtmmwlefuj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cashguo.top/gtabdbdezn.html

[R51] 排序去重取前几
来源：http://hz.yonumen.top/gtrnwcmixl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.pycfn.com/gtgjquzfxx.html

[R52] 统计行数
来源：http://hz.aizwys.cn/gtcodkmjkc.html

wc -l a.txt
来源：http://hz.xziqi.cn/gtkepdikkk.html

[R53] 查看文件头与实时尾
来源：http://hz.guowangkeji.top/gtfrkqqblq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gtsnkcbhbm.html

[R54] 比较两个文件
来源：http://hz.hysaishi.cn/gtfjgepkce.html

diff a.txt b.txt
来源：http://hz.chenjidiqi.icu/gthbtxyfhw.html

[R55] 压缩与解压
来源：http://hz.guannengcc.top/gturhtezob.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tian-w.cn/gthqtfyqjh.html

[R56] 远程拷贝
来源：http://hz.zhengqikj.top/gtwkvdmifs.html

scp file user@host:/path/
来源：http://hz.bjfxy.top/gtinsxrumh.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtmtzjzsih.html

ssh user@host 'uptime'
来源：http://hz.cdnleiting.top/gtcpkaspwe.html

[R58] 下载文件
来源：http://hz.hongshengwenyu.top/gtfjmyzdai.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.iojbl.cn/gtrwnyyhvr.html

[R59] 发 POST JSON
来源：http://hz.yuxming.cn/gtelixfpox.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangkeji.top/gtikfdtsis.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangdashe.top/gtocpghepe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenlongwang.top/gtgkldtkwr.html

[R61] 磁盘占用
来源：http://hz.svipenyu.cn/gtrkgosbvh.html

df -h;  du -sh *
来源：http://hz.bjfxy.top/gtwktnwlpm.html

[R62] 找最占空间的文件
来源：http://hz.quarkkingdee.top/gtcobwpxoc.html

du -ah . | sort -rh | head -10
来源：http://hz.tianlin.xyz/gteoujenql.html

[R63] 内存与进程
来源：http://hz.hfpthk.cn/gtefmibhzk.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gtrrsfcfne.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtgebatluw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ppjwa.cn/gtddgndnvq.html

[R65] 查看端口占用
来源：http://hz.316326.xyz/gtzyrqookd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sufxvd.cn/gtewibzjhi.html

[R66] 定时任务
来源：http://hz.yangfankeji.com/gtwdcmfpwp.html

crontab -e;  crontab -l
来源：http://hz.jinyuanbaomall.cn/gtmidizfph.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258888.top/gtsfeovwai.html

openssl rand -hex 16
来源：http://hz.jinqigfzy.top/gtpmbxmegu.html

[R68] 计算文件校验值
来源：http://hz.nanxuanxn.top/gtabxzcjhu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.wangdashe.top/gtdgfcrtao.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtcmbutwqn.html

head -c 16 /dev/urandom | base64
来源：http://hz.cucudq.cn/gtxpyhyzwz.html

[R70] 时间戳与互转
来源：http://hz.cheryme.top/gtqwzuyixy.html

date +%s;  date -d @1700000000
来源：http://hz.svipenyu.cn/gtdrhqpbwn.html

[R71] 日期格式化
来源：http://hz.mhx1999.top/gtdoboybdm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.birdmap.top/gtgivmuywq.html

[R72] 等待端口就绪
来源：http://hz.hnxiangtu.top/gtodkgkksa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.dashuyun.cn/gtwnagycyg.html

[R73] 分割大日志
来源：http://hz.jlsjyb.cn/gtjygjpboq.html

split -l 1000 big.log part_
来源：http://hz.cheryme.top/gttdmlzbsa.html

[R74] 批量重命名
来源：http://hz.mhx1999.top/gtkwaqbwoj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guannengcc.top/gtgmmdouly.html

[R75] 导出环境变量
来源：http://hz.bjfxy.top/gtrtmuldfj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xingfuxueyuan.xyz/gtqnrohins.html

[R76] 使用临时文件
来源：http://hz.xinyue.icu/gtavldrjbi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgufenzy.top/gtogrjawpw.html

[R77] 读取用户输入
来源：http://hz.yvedp.cn/gtmqmjjghb.html

read -rp "请输入: " ans
来源：http://hz.hnqzz.top/gtnhzqcukp.html

[R78] 交互式菜单
来源：http://hz.xinyue.icu/gtrdhjazkc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cucudq.cn/gtyhzkuxwz.html

[R79] 解析命令行选项
来源：http://hz.chenlongwang.top/gtoljwvhlg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pycfn.com/gtxoaqzivh.html

[R80] 查看脚本执行耗时
来源：http://hz.cashguo.top/gtilhlccip.html

time ./run.sh
来源：http://hz.daxiang520.top/gtpvxdtvum.html

================================================================================
来源：http://hz.jinqigufen.top/gtrpxcqfgm.html

S. C / C++ 专题
来源：http://hz.dashuyun.cn/gtuqneutbz.html

================================================================================
来源：http://hz.cdnleiting.top/gtzhrqcrzm.html

[S01] C：Hello World
来源：http://hz.9152youxi.cn/gtzonnritx.html

#include <stdio.h>
来源：http://hz.shanyushiyangkeji.top/gtpyuszgvs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yvedp.cn/gtqghjjdqk.html

[S02] C：变量与格式化输出
来源：http://hz.wangdashe.top/gtqsainfqg.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhengqikj.top/gtlyyneutq.html

[S03] C：读入整数
来源：http://hz.tianlin.xyz/gtxjwbogvn.html

int x; scanf("%d", &x);
来源：http://hz.guowangkeji.top/gtqqtogndk.html

[S04] C：字符串复制
来源：http://hz.cqqwz.cn/gtnbtcvtix.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.birdmap.top/gtuspadttq.html

[S05] C：字符串长度
来源：http://hz.haohaochexian.top/gtwjanefos.html

strlen(s)
来源：http://hz.ywan-chungtsiang.top/gtdvhwbaeo.html

[S06] C：字符串比较
来源：http://hz.xylfe.cn/gtcjzoirfp.html

strcmp(a, b) == 0
来源：http://hz.cdnleiting.top/gtxatpnfbx.html

[S07] C：数组遍历求和
来源：http://hz.yj20258888.top/gtnynjuuom.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xylfe.cn/gtlyroizzi.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangkeji.top/gtriowirna.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gogol.net.cn/gtwrxiqxcv.html

[S09] C：结构体定义与初始化
来源：http://hz.ywan-chungtsiang.top/gtlzqimkhs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.redwolf501.top/gtotggaleh.html

[S10] C：指针与解引用
来源：http://hz.bjfxy.top/gtihopcfdl.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtiyjxefoq.html

[S11] C：逐行读文件
来源：http://hz.ydjk.org.cn/gtfmtfwfkq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tanke756.top/gttvppwuxu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj202588.top/gtvjewzbzi.html

fclose(f);
来源：http://hz.hfpthk.cn/gtioikmnrm.html

[S12] C：写文件
来源：http://hz.aizwys.cn/gtpcgpqvcc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.52xcode.cn/gtjrlcvhuj.html

[S13] C：宏定义
来源：http://hz.nwbrower.top/gtqavuxigl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenzaomai.com/gtxtwtaojj.html

[S14] C：枚举
来源：http://hz.sxryk.cn/gtdryixrrv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.wangdashe.top/gtwsmvpycw.html

[S15] C：类型转换
来源：http://hz.ybcxt.top/gtxphqickk.html

(double) a / b
来源：http://hz.daria6918.cn/gtyywqtnfv.html

[S16] C：位操作置位
来源：http://hz.jinqigufen.top/gtzhttxshz.html

x |= (1 << 3);
来源：http://hz.chenlongwang.top/gtiouffnwo.html

[S17] C：安全拼接字符串
来源：http://hz.sufxvd.cn/gtuoqqmnvk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj20258.top/gtpdwsaaxe.html

[S18] C：命令行参数
来源：http://hz.chenjidiqi.icu/gtcwbfuzqr.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gtqwbxodvw.html

[S19] C：快速排序
来源：http://hz.tian-w.cn/gtfqaooreg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtfxgqplgw.html

[S20] C：二分查找
来源：http://hz.chenlongwang.top/gtlvtudtfg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtquowwumo.html

[S21] C：字符类别判断
来源：http://hz.chenjidiqi.icu/gtfomsirbk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhiwuduotai.top/gtasllehtr.html

[S22] C：字符串转数字
来源：http://hz.yvedp.cn/gtjwkpxjyx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.fengsongda.top/gtwvpeqsqy.html

[S23] C：随机数
来源：http://hz.ydjk.org.cn/gtgkbdpanf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xinyue.icu/gtnaprcklb.html

[S24] C：获取本地时间
来源：http://hz.52xcode.cn/gtzhnzqxzf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jlsjyb.cn/gtbhpdndkw.html

[S25] C：内存拷贝
来源：http://hz.dianchejie.cn/gtrvmxbhnk.html

memcpy(dst, src, n);
来源：http://hz.pycfn.com/gtanaaoqtb.html

[S26] C：内存清零
来源：http://hz.aizwys.cn/gtatvsnwtw.html

memset(a, 0, sizeof a);
来源：http://hz.daxiang520.top/gtqohrrsop.html

[S27] C：定义常量
来源：http://hz.jqgfzy.top/gtgqbenect.html

const double PI = 3.14159;
来源：http://hz.yvedp.cn/gtmfivnvdb.html

[S28] C：静态变量
来源：http://hz.jinqigufen.top/gtfytbjtqx.html

static int counter = 0;
来源：http://hz.wangdashe.top/gtlhavgaqf.html

[S29] C：变参函数
来源：http://hz.yonumen.top/gtoyszbqlh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydjk.org.cn/gtjrwzaagm.html

[S30] C：头文件保护
来源：http://hz.zhengqikj.top/gtbhupdlcb.html

#ifndef X_H
来源：http://hz.shuidangran.top/gtsiwzdkeq.html

#define X_H
来源：http://hz.smart0.xyz/gtzxffezav.html

#endif
来源：http://hz.yongpay.top/gtehdairox.html

[S31] C++：Hello World
来源：http://hz.xuanzx.com/gtdhbqoqor.html

#include <iostream>
来源：http://hz.shzxlz.cn/gtvzkbsmru.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gaohongyu789.top/gtbpwbrbie.html

[S32] C++：字符串
来源：http://hz.fengsongda.top/gtrtkmjgos.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258.top/gtsseetnud.html

[S33] C++：vector 增删
来源：http://hz.yangfankeji.com/gtqkvvsgez.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jianghu66.top/gtdyigennm.html

[S34] C++：遍历 vector
来源：http://hz.ehwqpu.com/gtkqhbvtku.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.bjfxy.top/gtxwkfxirw.html

[S35] C++：map
来源：http://hz.tian-w.cn/gthvdyqxdg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhengqikj.top/gtkumzenky.html

[S36] C++：unordered_map
来源：http://hz.zhijiandao.cn/gtreyzoesx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gtavcfjqol.html


<!-- 参考信息 -->