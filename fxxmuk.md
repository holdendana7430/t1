代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.316326.xyz/gtuidrdidl.html

[Q54] 清空表
来源：http://hz.9152youxi.cn/gtgdbrcgrm.html

TRUNCATE TABLE logs;
来源：http://hz.meibo888.top/gtxcodnmih.html

[Q55] 排名（并列占位）
来源：http://hz.hfpthk.cn/gtwkheqjoc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.xinyue.icu/gtydmsssjc.html

[Q56] 密集排名（并列不占位）
来源：http://hz.feifeiyinyue.top/gtlyonxswp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hnxiangtu.top/gtjioeqksm.html

[Q57] 行号
来源：http://hz.hywenlv.cn/gtyqxkxdrr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.daxiang520.top/gtiqqgeybr.html

[Q58] 累计求和
来源：http://hz.jyoumei.cn/gtjescsmvv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangdashe.top/gtgfumtyyd.html

[Q59] 分组内累计
来源：http://hz.zhoulong.xyz/gtmcnxtylb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.jqgfzy.top/gtemufgypo.html

[Q60] 取上一行 / 下一行
来源：http://hz.yj20258888.top/gttzsgejbj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ybcxt.top/gtbjeoefzu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.tian-w.cn/gtlwsbmioo.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtlpvbwhxf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.snrcjt.cn/gtptolxdme.html

[Q62] 分组占比
来源：http://hz.birdmap.top/gtikgbjxat.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zdqjudy.top/gtdfxoeagx.html

[Q63] 开启事务
来源：http://hz.chenzaomai.com/gtwjmeaxwh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xuanzx.com/gtdwsvsmvv.html

[Q64] 提交事务
来源：http://hz.pengpengdd.cyou/gtvczijnqu.html

COMMIT;
来源：http://hz.yj20258.top/gtqijbmump.html

[Q65] 回滚事务
来源：http://hz.zhongyouzk.top/gtscquigsb.html

ROLLBACK;
来源：http://hz.gogol.net.cn/gtqxfdzrvw.html

[Q66] 行锁查询
来源：http://hz.chenjidiqi.icu/gtpzuhuqok.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hnxiangtu.top/gtqhkgakmj.html

[Q67] 设置隔离级别
来源：http://hz.c1oappe.top/gthctjpqqy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yongpay.top/gtrsoqlsmu.html

[Q68] 保存点
来源：http://hz.guannengcc.top/gtmpqxlpte.html

SAVEPOINT sp1;
来源：http://hz.vqdsnc.cn/gtwyrclmgc.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangkeji.top/gtqehjuxvs.html

[Q69] 查看执行计划
来源：http://hz.jiagoushi.top/gtkykgarvv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.nwbrower.top/gtygebtvex.html

[Q70] 更新统计信息
来源：http://hz.mhx1999.top/gtbxwuiole.html

ANALYZE TABLE users;
来源：http://hz.guannengcc.top/gthgrfzjvx.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtzpyutpit.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.cqqwz.cn/gtslyyksrg.html

[Q72] 查看索引
来源：http://hz.ppjwa.cn/gtddhptdnu.html

SHOW INDEX FROM users;
来源：http://hz.yuxming.cn/gtnuvqrmig.html

[Q73] 查看表状态
来源：http://hz.yuxming.cn/gteanbcdjm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.guannengcc.top/gtgbejddjm.html

[Q74] 强制使用索引
来源：http://hz.cashguo.top/gtwzsrpgga.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gtlmpdgwbx.html

[Q75] 日期格式化
来源：http://hz.gaohongyu789.top/gtmqtxtnou.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shzxlz.cn/gtvvvvleim.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gtbrmaprfd.html

[Q76] 按天统计
来源：http://hz.hysaishi.cn/gtezynbrpt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shangyingyoupin.top/gtrdanjnzx.html

[Q77] 时间加减
来源：http://hz.zycfv.cn/gtilozftun.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.cucudq.cn/gtgckixngj.html

[Q78] 当前时间
来源：http://hz.cheryme.top/gtxouscxux.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.wangshuangyany.cn/gtpmjazswf.html

[Q79] 字符串拼接
来源：http://hz.aizwys.cn/gtdrkdriru.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.daria6918.cn/gtumrtmviw.html

[Q80] 字符串截取
来源：http://hz.ppjwa.cn/gtvezcljrr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenlongwang.top/gtelmvlsyv.html

[Q81] 字符串替换
来源：http://hz.iojbl.cn/gtgxlvdjky.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.chenjidiqi.icu/gtdkrdttju.html

[Q82] 字符长度与字节长度
来源：http://hz.cheryme.top/gtudedhmcl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tian-w.cn/gtcrvrwvlc.html

[Q83] 大小写转换
来源：http://hz.sweek.top/gtasomrrze.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yangfankeji.com/gtxljheigy.html

[Q84] 去除首尾空格
来源：http://hz.haohaochexian.top/gtjduuebjp.html

SELECT TRIM(name) FROM users;
来源：http://hz.jianghu66.top/gtkjgfunfn.html

[Q85] 数值取整
来源：http://hz.zdqjudy.top/gtwidbgwyj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sysykeji.top/gteqrxgbwm.html

[Q86] 读取 JSON 字段
来源：http://hz.feifeiyinyue.top/gtlogepobu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shzxlz.cn/gtppjzdhks.html

[Q87] JSON 字段做条件
来源：http://hz.gaohongyu789.top/gtuhlzrbjz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.birdmap.top/gtkiecfhna.html

[Q88] 行转列（条件聚合）
来源：http://hz.aizwys.cn/gtlxyxeoyf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yj202588.top/gtfewcmhby.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jianghu66.top/gtogeqwnvo.html

[Q89] 判断表是否存在
来源：http://hz.zhengqikj.top/gtospnpnzz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shanyushiyangkeji.top/gtwuentzkv.html

[Q90] 生成序号列
来源：http://hz.vqdsnc.cn/gtqsreoxjj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuetiantiany.cn/gtqsuxgiqz.html

================================================================================
来源：http://hz.xziqi.cn/gtxqahmahz.html

R. Bash 专题
来源：http://hz.zhixingplan.top/gtuuyiukir.html

================================================================================
来源：http://hz.haohaochexian.top/gtuwyccbef.html

[R01] shebang 与严格模式
来源：http://hz.snrcjt.cn/gtowricwhs.html

#!/usr/bin/env bash
来源：http://hz.sysykeji.top/gtmwrwmulk.html

set -euo pipefail
来源：http://hz.zhongyouzk.top/gtkdrilbbs.html

[R02] 变量赋值与使用
来源：http://hz.tanke756.top/gtwadiispy.html

name="Tom"; echo "$name"
来源：http://hz.cashguo.top/gtmsstcahy.html

[R03] 只读变量
来源：http://hz.xuetiantiany.cn/gtppukhuxa.html

readonly PI=3.14
来源：http://hz.hnxiangtu.top/gtbubhiwce.html

[R04] 位置参数
来源：http://hz.zycfv.cn/gtetrwiqbk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangshuangyany.cn/gtioiolzus.html

[R05] 参数默认值
来源：http://hz.yj202588.top/gttghlhhmx.html

name="${1:-default}"
来源：http://hz.tian-w.cn/gtwlluiggy.html

[R06] 判断命令是否存在
来源：http://hz.mhx1999.top/gtzhhivltr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenlongwang.top/gtqbnspbtk.html

[R07] if 判断文件
来源：http://hz.shanyushiyangkeji.top/gtzdbdonaw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gzhubu.top/gtdmutnssq.html

[R08] 数值比较
来源：http://hz.yongpay.top/gtakvftwke.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jlsjyb.cn/gtjmjpexws.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gtjqdmzbnw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtkbtcrmwq.html

[R10] 正则匹配
来源：http://hz.yonumen.top/gtcjjhhbld.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.pycfn.com/gtxmawllmv.html

[R11] case 多分支
来源：http://hz.guannengcc.top/gthqcvtqdq.html

case "$1" in
来源：http://hz.316326.xyz/gtkepgbnxz.html

start) echo "启动" ;;
来源：http://hz.c1oappe.top/gtaolokish.html

stop)  echo "停止" ;;
来源：http://hz.haohaochexian.top/gtpkvtnufy.html

*)     echo "未知命令" ;;
来源：http://hz.haohaochexian.top/gtsycrgibf.html

esac
来源：http://hz.yongpay.top/gtotcsnyjo.html

[R12] for 遍历文件
来源：http://hz.redwolf501.top/gtivjrxbfp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gaohongyu789.top/gtdotyvsbw.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtqrcbvzbu.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shzxlz.cn/gtldruhbjd.html

[R14] C 风格 for
来源：http://hz.cashguo.top/gtpmipqxnb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ydjk.org.cn/gtjshjdhdx.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtuhmftvdl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenzaomai.com/gtyvjtxpqs.html

[R16] until 等待条件
来源：http://hz.hfpthk.cn/gtqecpkvmw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gotoacloud.top/gtvetnkmgn.html

[R17] 数组定义与取值
来源：http://hz.zhoulong.xyz/gtsxjwndrd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yongpay.top/gtniccekbg.html

[R18] 遍历数组
来源：http://hz.gotoacloud.top/gtklfpazjq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.wangshuangyany.cn/gtkqogmapd.html

[R19] 数组长度
来源：http://hz.vqdsnc.cn/gtsflmeedu.html

echo "${#arr[@]}"
来源：http://hz.hnxiangtu.top/gthvspfmhi.html

[R20] 关联数组（字典）
来源：http://hz.jyoumei.cn/gtxyrrrugv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.quarkkingdee.top/gtzjvaroyc.html

[R21] 字符串长度
来源：http://hz.chenjidiqi.icu/gtpdslbgzg.html

echo "${#s}"
来源：http://hz.ppjwa.cn/gthtwclebn.html

[R22] 截取子串
来源：http://hz.yj202588.top/gtsuojfkvt.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gtbhrtqeul.html

[R23] 字符串替换
来源：http://hz.haohaochexian.top/gtkoanmmtu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shzxlz.cn/gtfcdhbwmg.html

[R24] 大小写转换
来源：http://hz.ydzc1.top/gtkdeccsoe.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenzaomai.com/gtbepytiqw.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgfzy.top/gtbpxxaixu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ppjwa.cn/gtucyrsulk.html

[R26] 命令替换
来源：http://hz.birdmap.top/gtpnumnffg.html

now=$(date +%F); echo "$now"
来源：http://hz.vqdsnc.cn/gtqgsianta.html

[R27] 算术展开
来源：http://hz.wangshuangyany.cn/gtuzpiuvrw.html

echo $((1 + 2 * 3))
来源：http://hz.shuidangran.top/gthuvhgtwh.html

[R28] 浮点运算
来源：http://hz.snrcjt.cn/gtxspysqan.html

echo "scale=2; 10/3" | bc
来源：http://hz.dashuyun.cn/gtjryaukyr.html

[R29] 定义函数
来源：http://hz.zycfv.cn/gtyjhsciqi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnqzz.top/gtxsrlcpai.html

[R30] 函数返回状态码
来源：http://hz.zhoulong.xyz/gtwmmsulmb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xingfuxueyuan.xyz/gtmffkjlxf.html

[R31] 局部变量
来源：http://hz.yvedp.cn/gteeqwgucz.html

f() { local x=1; echo "$x"; }
来源：http://hz.andypj.xyz/gtvivcbmpq.html

[R32] 参数个数校验
来源：http://hz.haohaochexian.top/gtmtkiycnj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.wangdashe.top/gtafatjbzf.html

[R33] 捕获错误并提示行号
来源：http://hz.yuxming.cn/gtisbvhsmp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aizwys.cn/gtnnygcfes.html

[R34] 退出时清理
来源：http://hz.yj20258888.top/gtutiqzwin.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtaevcxwsw.html

[R35] 后台执行并等待
来源：http://hz.nanxuanxn.top/gtbeopjjjr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.daria6918.cn/gtsmqxcsfq.html

[R36] 并发执行多个任务
来源：http://hz.chenzaomai.com/gtgpnlshqr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhiwuduotai.top/gtjnxnsczg.html

[R37] 把输出赋给变量
来源：http://hz.yanxiufei.cn/gtdozpzhyh.html

files=$(ls -1)
来源：http://hz.jianghu66.top/gtelceukpv.html

[R38] 管道串联
来源：http://hz.zhijiandao.cn/gtsohladjb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ywan-chungtsiang.top/gtxxgjgjwf.html

[R39] 重定向标准输出与错误
来源：http://hz.jianghu66.top/gtbrzgxmcs.html

cmd > out.log 2>&1
来源：http://hz.yonumen.top/gtixlcgmdx.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtvrdxxrqc.html

echo "log" >> out.log
来源：http://hz.yuxming.cn/gtknefbwdo.html

[R41] 丢弃输出
来源：http://hz.jinqigfzy.top/gtnmobfcto.html

cmd >/dev/null 2>&1
来源：http://hz.svipenyu.cn/gtpocxhevh.html

[R42] 输入重定向
来源：http://hz.shanyushiyangkeji.top/gteaxlmkta.html

wc -l < a.txt
来源：http://hz.guowangkeji.top/gtxnxdhral.html

[R43] 按名字查找文件
来源：http://hz.shuidangran.top/gtsgilrghp.html

find . -name "*.log" -type f
来源：http://hz.yj202588.top/gtjjojtwmm.html

[R44] 按修改时间查找
来源：http://hz.havefunace.top/gtsevaxdsj.html

find . -mtime -7 -type f
来源：http://hz.xylfe.cn/gtiarxiant.html

[R45] 批量删除
来源：http://hz.jinqigufen.top/gtxwnfbwgu.html

find . -name "*.tmp" -delete
来源：http://hz.dashuyun.cn/gthofdcnft.html

[R46] 递归替换文件内容
来源：http://hz.hfpthk.cn/gtxajitmah.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.xinyue.icu/gttoufvqwf.html

[R47] sed 单行替换
来源：http://hz.chenjidiqi.icu/gtnguommxd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aibaodan.cn/gtcgxqjfyj.html

[R48] awk 取指定列
来源：http://hz.tianlin.xyz/gtpbawgopn.html

awk '{print $1, $3}' a.txt
来源：http://hz.hongshengwenyu.top/gteqteqplf.html

[R49] awk 带条件
来源：http://hz.vqdsnc.cn/gtgdbkehiy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.mhx1999.top/gtkiyqqhzs.html

[R50] awk 求和
来源：http://hz.gotoacloud.top/gtywjlhjdw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yueranfly.top/gthlcylxfr.html

[R51] 排序去重取前几
来源：http://hz.xuetiantiany.cn/gtuojzdxyj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.quarkkingdee.top/gtcbnwvycd.html

[R52] 统计行数
来源：http://hz.ivvv.top/gtxfqbkwyi.html

wc -l a.txt
来源：http://hz.0kj1m.cn/gtcnbptblv.html

[R53] 查看文件头与实时尾
来源：http://hz.snrcjt.cn/gtjkqqcaid.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yj202588.top/gtpzihgmht.html

[R54] 比较两个文件
来源：http://hz.tianlin.xyz/gtmilcwtul.html

diff a.txt b.txt
来源：http://hz.yongpay.top/gtluqclfbr.html

[R55] 压缩与解压
来源：http://hz.zhixingplan.top/gtldydfieu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xingfuxueyuan.xyz/gtmlflgfqu.html

[R56] 远程拷贝
来源：http://hz.nwbrower.top/gtxbcyblys.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gtgzxeijbs.html

[R57] 远程执行命令
来源：http://hz.jqgfzy.top/gticrwvldt.html

ssh user@host 'uptime'
来源：http://hz.havefunace.top/gtjylsvdch.html

[R58] 下载文件
来源：http://hz.zycfv.cn/gtvohuysnh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xylfe.cn/gtfnknzncv.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gttkpypoyl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xylfe.cn/gtgbjjuchg.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtirkehbvp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xinyue.icu/gtqeaqpvbx.html

[R61] 磁盘占用
来源：http://hz.yj202588.top/gtyeiobxog.html

df -h;  du -sh *
来源：http://hz.pycfn.com/gtrayjqcqy.html

[R62] 找最占空间的文件
来源：http://hz.cashguo.top/gtmsxstpsb.html

du -ah . | sort -rh | head -10
来源：http://hz.gotoacloud.top/gtukfjjsxl.html

[R63] 内存与进程
来源：http://hz.fzhhl.top/gtrinbarzi.html

free -h;  ps aux | grep nginx
来源：http://hz.yangfankeji.com/gtflueznnw.html

[R64] 结束进程
来源：http://hz.gaohongyu789.top/gtqghqlubu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.dashuyun.cn/gtcecwpses.html

[R65] 查看端口占用
来源：http://hz.jinqigufen.top/gtesjeijko.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aibaodan.cn/gtbqquujjn.html

[R66] 定时任务
来源：http://hz.daxiang520.top/gtzgwcqlgv.html

crontab -e;  crontab -l
来源：http://hz.ydjk.org.cn/gtgadajazw.html

[R67] 生成随机十六进制串
来源：http://hz.xuetiantiany.cn/gttwsfdita.html

openssl rand -hex 16
来源：http://hz.jinqigfzy.top/gtkvxgxmbu.html

[R68] 计算文件校验值
来源：http://hz.aibaodan.cn/gthivdneon.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shuidangran.top/gtshrkwmwm.html

[R69] 生成随机密码
来源：http://hz.aibaodan.cn/gtiybrqnpj.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnxiangtu.top/gtyivzkeos.html

[R70] 时间戳与互转
来源：http://hz.gotoacloud.top/gttjzxmool.html

date +%s;  date -d @1700000000
来源：http://hz.zhixingplan.top/gtoorcqipv.html

[R71] 日期格式化
来源：http://hz.wangdashe.top/gtwykucyxw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ybcxt.top/gtmxmommce.html

[R72] 等待端口就绪
来源：http://hz.fzhhl.top/gtkttwnrwu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cdnleiting.top/gtimvqndlo.html

[R73] 分割大日志
来源：http://hz.svipenyu.cn/gtmxfopjor.html

split -l 1000 big.log part_
来源：http://hz.pengpengdd.cyou/gtqhyghaiu.html

[R74] 批量重命名
来源：http://hz.pengpengdd.cyou/gtfhbvywwz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yueranfly.top/gtqehsuqyl.html

[R75] 导出环境变量
来源：http://hz.haohaochexian.top/gtwhrzgprb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhiwuduotai.top/gtohsetuvu.html

[R76] 使用临时文件
来源：http://hz.zhongyouzk.top/gtovxdvndb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gtketwwxab.html

[R77] 读取用户输入
来源：http://hz.sufxvd.cn/gtnfilqhft.html

read -rp "请输入: " ans
来源：http://hz.wangshuangyany.cn/gtcrtxilrh.html

[R78] 交互式菜单
来源：http://hz.yj20258888.top/gtrjaplakk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zdqjudy.top/gtqsqwwyhp.html

[R79] 解析命令行选项
来源：http://hz.zhengqikj.top/gtsaxcqtgq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhoulong.xyz/gtwjdwnwow.html

[R80] 查看脚本执行耗时
来源：http://hz.xylfe.cn/gtvbswmbha.html

time ./run.sh
来源：http://hz.cheryme.top/gtcygdqpco.html

================================================================================
来源：http://hz.hfpthk.cn/gtviajvlzp.html

S. C / C++ 专题
来源：http://hz.quarkkingdee.top/gtcxhyfhti.html

================================================================================
来源：http://hz.ydzc1.top/gtlefqdsmh.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gtsnkplpeq.html

#include <stdio.h>
来源：http://hz.zhijiandao.cn/gtjqeefydp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gaohongyu789.top/gtbegpobsg.html

[S02] C：变量与格式化输出
来源：http://hz.nanxinkj.top/gtiitsdkkl.html

int a = 10; printf("%d\n", a);
来源：http://hz.ppjwa.cn/gteftuzurd.html

[S03] C：读入整数
来源：http://hz.shanyushiyangkeji.top/gtijprfqpl.html

int x; scanf("%d", &x);
来源：http://hz.dashuyun.cn/gtiwpnthqr.html

[S04] C：字符串复制
来源：http://hz.haohaochexian.top/gtwlgoszon.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jiagoushi.top/gtpnepxmgz.html

[S05] C：字符串长度
来源：http://hz.meibo888.top/gtalnbrzyt.html

strlen(s)
来源：http://hz.pengpengdd.cyou/gtcmkikoix.html

[S06] C：字符串比较
来源：http://hz.yanxiufei.cn/gtktjkqtjw.html

strcmp(a, b) == 0
来源：http://hz.wangshuangyany.cn/gttoxsjxpy.html

[S07] C：数组遍历求和
来源：http://hz.jyoumei.cn/gtelznlwwe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtqsikexll.html

[S08] C：动态内存分配与释放
来源：http://hz.guowangkeji.top/gtpzyznnjo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuanzhike.top/gtfmyuhqbt.html

[S09] C：结构体定义与初始化
来源：http://hz.bjfxy.top/gtbsqvsmrv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhongyouzk.top/gtaahjbryi.html

[S10] C：指针与解引用
来源：http://hz.kuanghao11.cn/gtovmlsfyk.html

int *p = &a;  *p = 5;
来源：http://hz.nwbrower.top/gtmsxlsnyp.html

[S11] C：逐行读文件
来源：http://hz.vqdsnc.cn/gttmxaqiyy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgfzy.top/gtilpyeghf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ybcxt.top/gtwzypnlbf.html

fclose(f);
来源：http://hz.sufxvd.cn/gtwsdoemsu.html

[S12] C：写文件
来源：http://hz.c1oappe.top/gtnksjfltb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hongshengwenyu.top/gtkosgwyns.html

[S13] C：宏定义
来源：http://hz.ybcxt.top/gttpgtkydn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtwhxpwvmo.html

[S14] C：枚举
来源：http://hz.xylfe.cn/gtmzueaswf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jyoumei.cn/gtjjylbrlg.html

[S15] C：类型转换
来源：http://hz.wangshuangyany.cn/gtooiawwuu.html

(double) a / b
来源：http://hz.gzhubu.top/gttzjafzwj.html

[S16] C：位操作置位
来源：http://hz.ppjwa.cn/gtuwlvkaqk.html

x |= (1 << 3);
来源：http://hz.shzxlz.cn/gtdnzzcmcn.html

[S17] C：安全拼接字符串
来源：http://hz.hfpthk.cn/gtvgkayqad.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgfzy.top/gtialtjfff.html

[S18] C：命令行参数
来源：http://hz.dashuyun.cn/gtivqhymco.html

int main(int argc, char **argv)
来源：http://hz.yvedp.cn/gtedoxvaqm.html

[S19] C：快速排序
来源：http://hz.zhengqikj.top/gtdnhnxmru.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtqhpamrqm.html

[S20] C：二分查找
来源：http://hz.yonumen.top/gtgjsdxsfl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgufenzy.top/gtawebjyzk.html

[S21] C：字符类别判断
来源：http://hz.meibo888.top/gtqxcxdnvm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yanxiufei.cn/gtkqovmgrv.html

[S22] C：字符串转数字
来源：http://hz.cashguo.top/gtfjuotswz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenzaomai.com/gtfwlhtqih.html

[S23] C：随机数
来源：http://hz.quarkkingdee.top/gtzjouigns.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinghuilouyu.cn/gtbqschckv.html

[S24] C：获取本地时间
来源：http://hz.9152youxi.cn/gtbilipzzn.html


<!-- 参考信息 -->