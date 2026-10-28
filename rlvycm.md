代发 wailian999

[Q65] 回滚事务
来源：http://hz.nanxinkj.top/gthuoeyjfe.html

ROLLBACK;
来源：http://hz.shzxlz.cn/gtginpapgn.html

[Q66] 行锁查询
来源：http://hz.cqqwz.cn/gtxovaqfxo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gtkcgswvrs.html

[Q67] 设置隔离级别
来源：http://hz.yanxiufei.cn/gtbwqsrpbv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.iojbl.cn/gttwjstvyr.html

[Q68] 保存点
来源：http://hz.yj20258.top/gtptzcbygi.html

SAVEPOINT sp1;
来源：http://hz.ybcxt.top/gtucjdeehu.html

ROLLBACK TO sp1;
来源：http://hz.guannengcc.top/gtzywultsq.html

[Q69] 查看执行计划
来源：http://hz.yj20258.top/gtgfzynlpd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sysykeji.top/gtyddzxtup.html

[Q70] 更新统计信息
来源：http://hz.svipenyu.cn/gthwsxpiww.html

ANALYZE TABLE users;
来源：http://hz.snrcjt.cn/gtokovyokb.html

[Q71] 查看建表语句
来源：http://hz.wangshuangyany.cn/gtcawlizje.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.fengsongda.top/gtpmtlehrk.html

[Q72] 查看索引
来源：http://hz.redwolf501.top/gttdmdfcos.html

SHOW INDEX FROM users;
来源：http://hz.ywan-chungtsiang.top/gtdhsmyimg.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtdxalinbv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.daxiang520.top/gtaqfpfrgk.html

[Q74] 强制使用索引
来源：http://hz.shuidangran.top/gtgwzigyma.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yonumen.top/gtbhhjlszn.html

[Q75] 日期格式化
来源：http://hz.shanyushiyangtech.top/gthaaapgtc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj202588.top/gtxffuhagl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yonumen.top/gtrenmrzsk.html

[Q76] 按天统计
来源：http://hz.guowangkeji.top/gtzfccydys.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gotoacloud.top/gtgvukslga.html

[Q77] 时间加减
来源：http://hz.zhengqikj.top/gtklbtpkum.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtwzsgthzv.html

[Q78] 当前时间
来源：http://hz.svipenyu.cn/gtpjetmbcg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yj20258888.top/gtztmodltn.html

[Q79] 字符串拼接
来源：http://hz.guowangkeji.top/gtzjveenad.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jyoumei.cn/gtulapahzr.html

[Q80] 字符串截取
来源：http://hz.jlsjyb.cn/gtaorulbbt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.52xcode.cn/gtowlqkdjy.html

[Q81] 字符串替换
来源：http://hz.xziqi.cn/gtjdaktzam.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yongpay.top/gtrnyatvls.html

[Q82] 字符长度与字节长度
来源：http://hz.zdqjudy.top/gtjawbsarm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jinqigufen.top/gtdsovvcae.html

[Q83] 大小写转换
来源：http://hz.zhijiandao.cn/gtfndsleep.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.kuanghao11.cn/gtqcmbofbb.html

[Q84] 去除首尾空格
来源：http://hz.shzxlz.cn/gtvmxsslsh.html

SELECT TRIM(name) FROM users;
来源：http://hz.cashguo.top/gtspyocamn.html

[Q85] 数值取整
来源：http://hz.nanxinkj.top/gtuxukkizt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhixingplan.top/gtjekxnfjw.html

[Q86] 读取 JSON 字段
来源：http://hz.zhiwuduotai.top/gtemwideyj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xuetiantiany.cn/gtmutuwtap.html

[Q87] JSON 字段做条件
来源：http://hz.dianchejie.cn/gtgupwwqnn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenzaomai.com/gtgnuyphqi.html

[Q88] 行转列（条件聚合）
来源：http://hz.andypj.xyz/gtoingppca.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jyoumei.cn/gtogldgldt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj20258.top/gtomdrueab.html

[Q89] 判断表是否存在
来源：http://hz.jianghu66.top/gtqpdpuaqs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yj20258.top/gtwahzkwiq.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gtyzyrtiab.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.quarkkingdee.top/gtrgmetelo.html

================================================================================
来源：http://hz.c1oappe.top/gtviqzvmab.html

R. Bash 专题
来源：http://hz.xziqi.cn/gtvliamhtf.html

================================================================================
来源：http://hz.svipenyu.cn/gtsfnwntdk.html

[R01] shebang 与严格模式
来源：http://hz.cashguo.top/gtzhkocwyi.html

#!/usr/bin/env bash
来源：http://hz.hnxiangtu.top/gtfuwkmrzs.html

set -euo pipefail
来源：http://hz.yvedp.cn/gtuoczfoyk.html

[R02] 变量赋值与使用
来源：http://hz.haohaochexian.top/gtfkfnxaxe.html

name="Tom"; echo "$name"
来源：http://hz.hfpthk.cn/gtjhhkfrvk.html

[R03] 只读变量
来源：http://hz.shangyingyoupin.top/gtwnkjdwij.html

readonly PI=3.14
来源：http://hz.cqqwz.cn/gtnuckwqrn.html

[R04] 位置参数
来源：http://hz.tanke756.top/gtcauhitpp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jlsjyb.cn/gttrrnszui.html

[R05] 参数默认值
来源：http://hz.vqdsnc.cn/gttfxmhhxk.html

name="${1:-default}"
来源：http://hz.sysykeji.top/gtgrhhealx.html

[R06] 判断命令是否存在
来源：http://hz.yueranfly.top/gtargribbh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yongpay.top/gtpxegawad.html

[R07] if 判断文件
来源：http://hz.ydzc1.top/gtqodxvjii.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.daria6918.cn/gtcxygrlxk.html

[R08] 数值比较
来源：http://hz.meibo888.top/gtqtldbijx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuetiantiany.cn/gtrmxailxx.html

[R09] 字符串比较
来源：http://hz.zhongyouzk.top/gtzazynzlq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yueranfly.top/gtzkahtgae.html

[R10] 正则匹配
来源：http://hz.zycfv.cn/gtvzsurafh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtfbtwkesj.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gtmctvxtpy.html

case "$1" in
来源：http://hz.gotoacloud.top/gtobvcayoh.html

start) echo "启动" ;;
来源：http://hz.vqdsnc.cn/gtrajglttr.html

stop)  echo "停止" ;;
来源：http://hz.0kj1m.cn/gteypzyowk.html

*)     echo "未知命令" ;;
来源：http://hz.zhoulong.xyz/gtcrkcwken.html

esac
来源：http://hz.svipenyu.cn/gtpkbzktwf.html

[R12] for 遍历文件
来源：http://hz.jinyuanbaomall.cn/gthpijssdu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.iojbl.cn/gtulknkrmi.html

[R13] for 计数循环
来源：http://hz.wangshuangyany.cn/gtkoxkzitx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.quarkkingdee.top/gtdqvuznzv.html

[R14] C 风格 for
来源：http://hz.vqdsnc.cn/gtyptkzlrh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ybcxt.top/gtxpsbdyrd.html

[R15] while 逐行读文件
来源：http://hz.ppjwa.cn/gtykjsaxqd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgufenzy.top/gtzevfzegu.html

[R16] until 等待条件
来源：http://hz.yj20258888.top/gtpxfczulm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gogol.net.cn/gtbgiienxr.html

[R17] 数组定义与取值
来源：http://hz.xuetiantiany.cn/gtcfadlawy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sxryk.cn/gtxqnxphte.html

[R18] 遍历数组
来源：http://hz.zhijiandao.cn/gtansvztuv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shuidangran.top/gthipljkzf.html

[R19] 数组长度
来源：http://hz.yj202588.top/gtpzbtjhrs.html

echo "${#arr[@]}"
来源：http://hz.ydzc1.top/gtevayyecv.html

[R20] 关联数组（字典）
来源：http://hz.zhixingplan.top/gtxuerirat.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aibaodan.cn/gtapuxzquw.html

[R21] 字符串长度
来源：http://hz.xylfe.cn/gtehzzxvcw.html

echo "${#s}"
来源：http://hz.yj20258.top/gtrwjiahfs.html

[R22] 截取子串
来源：http://hz.xylfe.cn/gtfeoplibc.html

echo "${s:0:5}"
来源：http://hz.dianchejie.cn/gtzytqhyii.html

[R23] 字符串替换
来源：http://hz.yonumen.top/gtrajenimm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.fengsongda.top/gthnfsaukq.html

[R24] 大小写转换
来源：http://hz.gaohongyu789.top/gtfuhqemgb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cqqwz.cn/gtabzfwxmc.html

[R25] 去后缀 / 去前缀
来源：http://hz.ivvv.top/gttsazgonr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnxiangtu.top/gtffpdhekh.html

[R26] 命令替换
来源：http://hz.jinyuanbaomall.cn/gttlicobkc.html

now=$(date +%F); echo "$now"
来源：http://hz.tian-w.cn/gtgsgzvuna.html

[R27] 算术展开
来源：http://hz.jqgfzy.top/gtdxlfgfkv.html

echo $((1 + 2 * 3))
来源：http://hz.smart0.xyz/gtiwjqhtdc.html

[R28] 浮点运算
来源：http://hz.cheryme.top/gtmseucfve.html

echo "scale=2; 10/3" | bc
来源：http://hz.gotoacloud.top/gtuufoezok.html

[R29] 定义函数
来源：http://hz.redwolf501.top/gtyyhkslue.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuetiantiany.cn/gtuyskruvq.html

[R30] 函数返回状态码
来源：http://hz.ppjwa.cn/gtylwyqxxd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuanzhike.top/gtiilnevjt.html

[R31] 局部变量
来源：http://hz.xinyue.icu/gtuwuasirc.html

f() { local x=1; echo "$x"; }
来源：http://hz.c1oappe.top/gttgzruxzc.html

[R32] 参数个数校验
来源：http://hz.chenzaomai.com/gtssfgjnrf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sysykeji.top/gtnlvaoofe.html

[R33] 捕获错误并提示行号
来源：http://hz.ywan-chungtsiang.top/gthtvaumhz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tianlin.xyz/gtlqqoczlo.html

[R34] 退出时清理
来源：http://hz.bjfxy.top/gtntgmehtt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtyhgwwhfb.html

[R35] 后台执行并等待
来源：http://hz.birdmap.top/gtjbxqveck.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jlsjyb.cn/gtswyzcdxt.html

[R36] 并发执行多个任务
来源：http://hz.pycfn.com/gtxhmmmbsb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cdnleiting.top/gthimnctyw.html

[R37] 把输出赋给变量
来源：http://hz.nwbrower.top/gtwlrbsojc.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtcaoucqjq.html

[R38] 管道串联
来源：http://hz.ydzc1.top/gthxddztmq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jlsjyb.cn/gtdpcvvmhr.html

[R39] 重定向标准输出与错误
来源：http://hz.xylfe.cn/gtgmagsdhf.html

cmd > out.log 2>&1
来源：http://hz.cdnleiting.top/gtsumljpmd.html

[R40] 追加写日志
来源：http://hz.daria6918.cn/gtddfjvwgr.html

echo "log" >> out.log
来源：http://hz.9152youxi.cn/gtoaezvgyk.html

[R41] 丢弃输出
来源：http://hz.316326.xyz/gtjeuzvhlq.html

cmd >/dev/null 2>&1
来源：http://hz.smart0.xyz/gtiamcyzhx.html

[R42] 输入重定向
来源：http://hz.yongpay.top/gteazfbpgo.html

wc -l < a.txt
来源：http://hz.zhengqikj.top/gtjdlxkdvc.html

[R43] 按名字查找文件
来源：http://hz.cashguo.top/gtwcbrlhvg.html

find . -name "*.log" -type f
来源：http://hz.jinghuilouyu.cn/gtrzcxnebs.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangtech.top/gtnxawkhjy.html

find . -mtime -7 -type f
来源：http://hz.zdqjudy.top/gtjtpajhzv.html

[R45] 批量删除
来源：http://hz.zhijiandao.cn/gtqabsdvgg.html

find . -name "*.tmp" -delete
来源：http://hz.gotoacloud.top/gtwzcepyhq.html

[R46] 递归替换文件内容
来源：http://hz.zycfv.cn/gtxsfutcsc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxuanxn.top/gthkfllfws.html

[R47] sed 单行替换
来源：http://hz.gzhubu.top/gtdppylkim.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhixingplan.top/gtpdzdjiaz.html

[R48] awk 取指定列
来源：http://hz.daxiang520.top/gtupcvmmez.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxinkj.top/gtorxjaaeq.html

[R49] awk 带条件
来源：http://hz.yueranfly.top/gtuuxpyxnp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydzc1.top/gtihswrfrg.html

[R50] awk 求和
来源：http://hz.jinyuanbaomall.cn/gtoksfmuwv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ydjk.org.cn/gtwqcnnokt.html

[R51] 排序去重取前几
来源：http://hz.xziqi.cn/gthdzyqcpk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hywenlv.cn/gtypgrnvww.html

[R52] 统计行数
来源：http://hz.zhengqikj.top/gthvytgrmp.html

wc -l a.txt
来源：http://hz.pengpengdd.cyou/gtcdcwgdbm.html

[R53] 查看文件头与实时尾
来源：http://hz.bjfxy.top/gtohqmhwbj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hfpthk.cn/gtgzwzxdfc.html

[R54] 比较两个文件
来源：http://hz.wangdashe.top/gtfspqldaj.html

diff a.txt b.txt
来源：http://hz.jqgfzy.top/gtqyyrodtc.html

[R55] 压缩与解压
来源：http://hz.sweek.top/gtnmhjmgkw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shuidangran.top/gtjjbcmesi.html

[R56] 远程拷贝
来源：http://hz.jyoumei.cn/gtuofkslxl.html

scp file user@host:/path/
来源：http://hz.wangshuangyany.cn/gtgueaddjx.html

[R57] 远程执行命令
来源：http://hz.316326.xyz/gtyfiyeihe.html

ssh user@host 'uptime'
来源：http://hz.hammf.cn/gtkirkejij.html

[R58] 下载文件
来源：http://hz.ybcxt.top/gtdyetniaz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.quarkkingdee.top/gtwuuakhlr.html

[R59] 发 POST JSON
来源：http://hz.ivvv.top/gtgqxouptk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aizwys.cn/gtsldhywlp.html

[R60] 只看 HTTP 状态码
来源：http://hz.snrcjt.cn/gtjandfzeh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtalvtjsmw.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gttbqkjmtf.html

df -h;  du -sh *
来源：http://hz.shanyushiyangkeji.top/gtixqqxenn.html

[R62] 找最占空间的文件
来源：http://hz.52xcode.cn/gtoyakojxp.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gthcwcqloi.html

[R63] 内存与进程
来源：http://hz.yanxiufei.cn/gtlveopmel.html

free -h;  ps aux | grep nginx
来源：http://hz.hnxiangtu.top/gtwpmfzryr.html

[R64] 结束进程
来源：http://hz.0kj1m.cn/gtwjmaqzat.html

kill -9 $(pgrep -f app.py)
来源：http://hz.pengpengdd.cyou/gtvvwodhkq.html

[R65] 查看端口占用
来源：http://hz.pycfn.com/gtjovotveh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhijiandao.cn/gtboiqqdpw.html

[R66] 定时任务
来源：http://hz.zhengqikj.top/gtoplibwdp.html

crontab -e;  crontab -l
来源：http://hz.yj20258.top/gtrfvemaso.html

[R67] 生成随机十六进制串
来源：http://hz.yueranfly.top/gtvizdiqzk.html

openssl rand -hex 16
来源：http://hz.cheryme.top/gtygpznzaq.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtmllrfdpo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daria6918.cn/gtmkvsipja.html

[R69] 生成随机密码
来源：http://hz.fengsongda.top/gtlbmnlpvs.html

head -c 16 /dev/urandom | base64
来源：http://hz.aizwys.cn/gtjqelmbmk.html

[R70] 时间戳与互转
来源：http://hz.ywan-chungtsiang.top/gtiiwwmqin.html

date +%s;  date -d @1700000000
来源：http://hz.yj202588.top/gtxszmmrhs.html

[R71] 日期格式化
来源：http://hz.cdnleiting.top/gtbisvbdbe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ywan-chungtsiang.top/gtvdtgvbnv.html

[R72] 等待端口就绪
来源：http://hz.shzxlz.cn/gtattczlcf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tian-w.cn/gtomtgutox.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gthfnprksk.html

split -l 1000 big.log part_
来源：http://hz.pycfn.com/gtebpocspe.html

[R74] 批量重命名
来源：http://hz.zhixingplan.top/gttxmpuhst.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhongyouzk.top/gtrilogdyy.html

[R75] 导出环境变量
来源：http://hz.guowangkeji.top/gtkmryhfhs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xziqi.cn/gtubdbmqky.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtovrwvrff.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hfpthk.cn/gtypwblvbv.html

[R77] 读取用户输入
来源：http://hz.hammf.cn/gtijvfpyut.html

read -rp "请输入: " ans
来源：http://hz.hammf.cn/gtmlqfhreb.html

[R78] 交互式菜单
来源：http://hz.zhongyouzk.top/gtyumtchpm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xylfe.cn/gtrrlruifz.html

[R79] 解析命令行选项
来源：http://hz.jyoumei.cn/gtdjzsideg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.vqdsnc.cn/gtzralyfqe.html

[R80] 查看脚本执行耗时
来源：http://hz.fzhhl.top/gtmhejvglm.html

time ./run.sh
来源：http://hz.ehwqpu.com/gtuvkiyrco.html

================================================================================
来源：http://hz.jqgfzy.top/gthxkhsvdw.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gtzkecmasw.html

================================================================================
来源：http://hz.ybcxt.top/gtnpgstglw.html

[S01] C：Hello World
来源：http://hz.andypj.xyz/gtvyjitflc.html

#include <stdio.h>
来源：http://hz.yj202588.top/gtdpuzemat.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinghuilouyu.cn/gtxtvyavme.html

[S02] C：变量与格式化输出
来源：http://hz.yueranfly.top/gtccqtajwn.html

int a = 10; printf("%d\n", a);
来源：http://hz.tanke756.top/gtylswlmer.html

[S03] C：读入整数
来源：http://hz.feifeiyinyue.top/gtkpvfoqmh.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangkeji.top/gtyjnsyccn.html

[S04] C：字符串复制
来源：http://hz.cashguo.top/gthvjxgkfs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jqgfzy.top/gtfhlgtmds.html

[S05] C：字符串长度
来源：http://hz.zhixingplan.top/gtzsfvjnzf.html

strlen(s)
来源：http://hz.hnxiangtu.top/gtcanyvjqu.html

[S06] C：字符串比较
来源：http://hz.andypj.xyz/gtaxawbyvd.html

strcmp(a, b) == 0
来源：http://hz.ehwqpu.com/gtvpdxidvf.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtesgkiifn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.52xcode.cn/gtiqguitnr.html

[S08] C：动态内存分配与释放
来源：http://hz.fengsongda.top/gtzwjduhuv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.kuanghao11.cn/gtdvwmvjbc.html

[S09] C：结构体定义与初始化
来源：http://hz.sysykeji.top/gtsafmywtm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtkplichjx.html

[S10] C：指针与解引用
来源：http://hz.jianghu66.top/gteqgeetbu.html

int *p = &a;  *p = 5;
来源：http://hz.cashguo.top/gtcuxewbix.html

[S11] C：逐行读文件
来源：http://hz.zhengqikj.top/gtljnzmpqo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cdnleiting.top/gtithmxauj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhixingplan.top/gtlobztrjk.html

fclose(f);
来源：http://hz.hysaishi.cn/gtleeuaixc.html

[S12] C：写文件
来源：http://hz.hnqzz.top/gtdocwzbgo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jianghu66.top/gtetqtnkrz.html

[S13] C：宏定义
来源：http://hz.cdnleiting.top/gtrbfebbkb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guowangkeji.top/gtyvlgtwmu.html

[S14] C：枚举
来源：http://hz.zhijiandao.cn/gtirdgwprp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.svipenyu.cn/gtlztnighg.html

[S15] C：类型转换
来源：http://hz.yonumen.top/gthpyfxrld.html

(double) a / b
来源：http://hz.zhixingplan.top/gtbgksvmpd.html

[S16] C：位操作置位
来源：http://hz.tian-w.cn/gtpuftqboc.html

x |= (1 << 3);
来源：http://hz.tian-w.cn/gtuxvgmwjz.html

[S17] C：安全拼接字符串
来源：http://hz.redwolf501.top/gtdhpvxgzs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.feifeiyinyue.top/gtmkvlsaro.html

[S18] C：命令行参数
来源：http://hz.hongshengwenyu.top/gtojmscemr.html

int main(int argc, char **argv)
来源：http://hz.shzxlz.cn/gthtxivqss.html

[S19] C：快速排序
来源：http://hz.fengsongda.top/gtkpxmjrtd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jqgfzy.top/gtzllcexwy.html

[S20] C：二分查找
来源：http://hz.jinghuilouyu.cn/gtmrumsbka.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhijiandao.cn/gtbmelebdf.html

[S21] C：字符类别判断
来源：http://hz.chenlongwang.top/gtlhtlabdl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.guannengcc.top/gtxynpaccs.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtuihtklxz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenjidiqi.icu/gtdkamrats.html

[S23] C：随机数
来源：http://hz.wangshuangyany.cn/gtcesjvhvd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.birdmap.top/gtdmpmzapa.html

[S24] C：获取本地时间
来源：http://hz.xinyue.icu/gtmqghgltw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhijiandao.cn/gtybzbipcv.html

[S25] C：内存拷贝
来源：http://hz.fzhhl.top/gtxrjolscg.html

memcpy(dst, src, n);
来源：http://hz.svipenyu.cn/gtivdgujga.html

[S26] C：内存清零
来源：http://hz.ivvv.top/gtohjgjvzo.html

memset(a, 0, sizeof a);
来源：http://hz.nanxuanxn.top/gtabvlwtjl.html

[S27] C：定义常量
来源：http://hz.sweek.top/gtskapypss.html

const double PI = 3.14159;
来源：http://hz.jiagoushi.top/gttnawfate.html

[S28] C：静态变量
来源：http://hz.dashuyun.cn/gtxogkzyau.html

static int counter = 0;
来源：http://hz.hongshengwenyu.top/gtbnkdmsqm.html

[S29] C：变参函数
来源：http://hz.tianlin.xyz/gtlbdwxkbe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhiwuduotai.top/gtrrvhryvh.html

[S30] C：头文件保护
来源：http://hz.316326.xyz/gtzhzedest.html

#ifndef X_H
来源：http://hz.gzhubu.top/gtmpdlnjss.html

#define X_H
来源：http://hz.iojbl.cn/gtxggzpdmr.html

#endif
来源：http://hz.hfpthk.cn/gtyqwjmdtn.html

[S31] C++：Hello World
来源：http://hz.wangshuangyany.cn/gtfmrzdhtp.html

#include <iostream>
来源：http://hz.xuanzx.com/gtcyhrimil.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.smart0.xyz/gtbjltacnj.html

[S32] C++：字符串
来源：http://hz.hywenlv.cn/gtwslyxjwv.html

std::string s = "hi";  s += "!";
来源：http://hz.jianghu66.top/gtcpzaleqg.html

[S33] C++：vector 增删
来源：http://hz.feifeiyinyue.top/gtnrribbtj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.meibo888.top/gtdwbkpmre.html

[S34] C++：遍历 vector
来源：http://hz.meibo888.top/gtvvykkrbt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gthzfisnha.html


<!-- 参考信息 -->