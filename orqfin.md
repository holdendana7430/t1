代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinyuanbaomall.cn/gtehnzqqvq.html

[Q52] 删除指定行
来源：http://hz.yuanzhike.top/gtvjvlbbms.html

DELETE FROM users WHERE id = 10;
来源：http://hz.smart0.xyz/gttrvpgmcm.html

[Q53] 按条件删除
来源：http://hz.fengsongda.top/gtnsolzgie.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.chenlongwang.top/gtqazfqpfr.html

[Q54] 清空表
来源：http://hz.ppjwa.cn/gtuvjznpuy.html

TRUNCATE TABLE logs;
来源：http://hz.xingfuxueyuan.xyz/gtayailkaj.html

[Q55] 排名（并列占位）
来源：http://hz.yonumen.top/gthnylciab.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.fengsongda.top/gttegwhhvi.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ydzc1.top/gtcprpodup.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhongyouzk.top/gtwvwpmcwd.html

[Q57] 行号
来源：http://hz.cqqwz.cn/gtkasyvzio.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hfpthk.cn/gtfszpquox.html

[Q58] 累计求和
来源：http://hz.haohaochexian.top/gthbzqqddy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.316326.xyz/gtxugdgeza.html

[Q59] 分组内累计
来源：http://hz.chenzaomai.com/gtohjnxbsu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.bjfxy.top/gtegzmmcbv.html

[Q60] 取上一行 / 下一行
来源：http://hz.xylfe.cn/gtqyvfvtbp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zycfv.cn/gtwxxqyvfz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhengqikj.top/gtvgxndfts.html

[Q61] 移动平均
来源：http://hz.zhiwuduotai.top/gtjwzwxvyd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zdqjudy.top/gtfzekrrku.html

[Q62] 分组占比
来源：http://hz.zhongyouzk.top/gtegxtoubj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.mhx1999.top/gtljhnupvn.html

[Q63] 开启事务
来源：http://hz.sxryk.cn/gtogyqposk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ywan-chungtsiang.top/gtfblpdmns.html

[Q64] 提交事务
来源：http://hz.xuetiantiany.cn/gtktcqsabu.html

COMMIT;
来源：http://hz.feifeiyinyue.top/gtkeutxauu.html

[Q65] 回滚事务
来源：http://hz.dashuyun.cn/gtawhipmkf.html

ROLLBACK;
来源：http://hz.yonumen.top/gttiaidqva.html

[Q66] 行锁查询
来源：http://hz.wangshuangyany.cn/gtbfkevrll.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gtgnyywmso.html

[Q67] 设置隔离级别
来源：http://hz.havefunace.top/gtrptjngbx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.daria6918.cn/gtheutxoem.html

[Q68] 保存点
来源：http://hz.daxiang520.top/gtkvtgnnfs.html

SAVEPOINT sp1;
来源：http://hz.jinqigufen.top/gttwfffnpt.html

ROLLBACK TO sp1;
来源：http://hz.smart0.xyz/gtpvznmqsw.html

[Q69] 查看执行计划
来源：http://hz.yongpay.top/gthhffyabd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ppjwa.cn/gtclguyejn.html

[Q70] 更新统计信息
来源：http://hz.hywenlv.cn/gttusloyzl.html

ANALYZE TABLE users;
来源：http://hz.zhongyouzk.top/gtzsgbhhra.html

[Q71] 查看建表语句
来源：http://hz.gzhubu.top/gtqhpddyww.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenzaomai.com/gtoofqqzxp.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gtqahowgft.html

SHOW INDEX FROM users;
来源：http://hz.zhijiandao.cn/gtgcjfaqid.html

[Q73] 查看表状态
来源：http://hz.yanxiufei.cn/gthobesajg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sufxvd.cn/gtrlwxxdea.html

[Q74] 强制使用索引
来源：http://hz.52xcode.cn/gttazvfsen.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.dianchejie.cn/gtzbbwmklh.html

[Q75] 日期格式化
来源：http://hz.zdqjudy.top/gtrbppkido.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.mhx1999.top/gtgzermgzk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.ivvv.top/gtqoupmikh.html

[Q76] 按天统计
来源：http://hz.zhongyouzk.top/gtaaoqljqt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtwalhtvej.html

[Q77] 时间加减
来源：http://hz.nwbrower.top/gtmcaeqczh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.52xcode.cn/gtvrinawkx.html

[Q78] 当前时间
来源：http://hz.zhixingplan.top/gtvucuqxdr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.9152youxi.cn/gtjmbwjwqm.html

[Q79] 字符串拼接
来源：http://hz.xingfuxueyuan.xyz/gtcchbsfqp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nanxuanxn.top/gtiuljfmos.html

[Q80] 字符串截取
来源：http://hz.yangfankeji.com/gtacwkabud.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sufxvd.cn/gtykwpzqie.html

[Q81] 字符串替换
来源：http://hz.fzhhl.top/gtbvpcymhv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.quarkkingdee.top/gtwhoffpcz.html

[Q82] 字符长度与字节长度
来源：http://hz.yongpay.top/gtbftivkhx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.guowangkeji.top/gtztnbidlp.html

[Q83] 大小写转换
来源：http://hz.gzhubu.top/gtjgbsqmsa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.daria6918.cn/gtfihzgghh.html

[Q84] 去除首尾空格
来源：http://hz.svipenyu.cn/gtmrgmwhpa.html

SELECT TRIM(name) FROM users;
来源：http://hz.316326.xyz/gtouvnygtq.html

[Q85] 数值取整
来源：http://hz.cqqwz.cn/gtybonvbhb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pengpengdd.cyou/gtqqmkzbkh.html

[Q86] 读取 JSON 字段
来源：http://hz.shanyushiyangkeji.top/gtuhgrznmm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hywenlv.cn/gtgdjfzskt.html

[Q87] JSON 字段做条件
来源：http://hz.bjfxy.top/gthpjqoabp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.quarkkingdee.top/gtvbmpqvjr.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhaomingkeji.xyz/gttwnmdxxh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sxryk.cn/gtiyxybyyz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.fengsongda.top/gtfaqzabzv.html

[Q89] 判断表是否存在
来源：http://hz.hnqzz.top/gtauboozxo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hongshengwenyu.top/gtsquduxul.html

[Q90] 生成序号列
来源：http://hz.hywenlv.cn/gtsauayxxw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtaoqbkusq.html

================================================================================
来源：http://hz.hnxiangtu.top/gtghiyhfch.html

R. Bash 专题
来源：http://hz.yueranfly.top/gtbbtsbhua.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtxqkdqwey.html

[R01] shebang 与严格模式
来源：http://hz.cdnleiting.top/gtcvucmcoq.html

#!/usr/bin/env bash
来源：http://hz.jinghuilouyu.cn/gteshslwei.html

set -euo pipefail
来源：http://hz.iojbl.cn/gtbluotyoo.html

[R02] 变量赋值与使用
来源：http://hz.chenjidiqi.icu/gtiurlpwer.html

name="Tom"; echo "$name"
来源：http://hz.aibaodan.cn/gtrpojjrfh.html

[R03] 只读变量
来源：http://hz.feifeiyinyue.top/gtquughoxa.html

readonly PI=3.14
来源：http://hz.chenlongwang.top/gtulggbhtc.html

[R04] 位置参数
来源：http://hz.bjfxy.top/gtepaaxlre.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangkeji.top/gtgxfiqwtk.html

[R05] 参数默认值
来源：http://hz.xingfuxueyuan.xyz/gtgdfdxupl.html

name="${1:-default}"
来源：http://hz.fengsongda.top/gtmghxcndu.html

[R06] 判断命令是否存在
来源：http://hz.nanxuanxn.top/gtsvqlzlrh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.haohaochexian.top/gtnrmonfxk.html

[R07] if 判断文件
来源：http://hz.shuidangran.top/gttoqzdudx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tian-w.cn/gtakffmyla.html

[R08] 数值比较
来源：http://hz.bjfxy.top/gtsxebidxm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuanzx.com/gtrxnwwsig.html

[R09] 字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtrqqddtgj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gogol.net.cn/gtaidykvgz.html

[R10] 正则匹配
来源：http://hz.gogol.net.cn/gtwqfcfrva.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtqlvsxrew.html

[R11] case 多分支
来源：http://hz.chenlongwang.top/gtbknvpmpt.html

case "$1" in
来源：http://hz.zhijiandao.cn/gtqujtooiz.html

start) echo "启动" ;;
来源：http://hz.jinqigfzy.top/gtkrqtnltx.html

stop)  echo "停止" ;;
来源：http://hz.hongshengwenyu.top/gtjpgqywex.html

*)     echo "未知命令" ;;
来源：http://hz.yvedp.cn/gtjhnrjorz.html

esac
来源：http://hz.xuetiantiany.cn/gtamiiyuwd.html

[R12] for 遍历文件
来源：http://hz.redwolf501.top/gtpgvmgfqf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnqzz.top/gtoiortcpk.html

[R13] for 计数循环
来源：http://hz.hongshengwenyu.top/gtzgyrunup.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.haohaochexian.top/gthunfitbz.html

[R14] C 风格 for
来源：http://hz.gaohongyu789.top/gtsfphqjuf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtmgwopsci.html

[R15] while 逐行读文件
来源：http://hz.iojbl.cn/gtjisfvwyk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinghuilouyu.cn/gtfjqmkank.html

[R16] until 等待条件
来源：http://hz.zhaomingkeji.xyz/gtyundzseq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zycfv.cn/gteyckvzmk.html

[R17] 数组定义与取值
来源：http://hz.zhengqikj.top/gtatwuobxc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhiwuduotai.top/gthstgothb.html

[R18] 遍历数组
来源：http://hz.hfpthk.cn/gtxoulzmmf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gtnhxqranf.html

[R19] 数组长度
来源：http://hz.redwolf501.top/gtrtnxltlo.html

echo "${#arr[@]}"
来源：http://hz.dianchejie.cn/gtccjvztqj.html

[R20] 关联数组（字典）
来源：http://hz.ivvv.top/gtizffnddo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ywan-chungtsiang.top/gtuzalsepb.html

[R21] 字符串长度
来源：http://hz.shzxlz.cn/gtgxhegosq.html

echo "${#s}"
来源：http://hz.yj20258.top/gtldgasuou.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtmhooowdf.html

echo "${s:0:5}"
来源：http://hz.hammf.cn/gtkeyxenop.html

[R23] 字符串替换
来源：http://hz.nanxuanxn.top/gteqfnbyhn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.meibo888.top/gtkhcojrkz.html

[R24] 大小写转换
来源：http://hz.chenjidiqi.icu/gtvsqtungf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pycfn.com/gttghyubfc.html

[R25] 去后缀 / 去前缀
来源：http://hz.iojbl.cn/gthqcehncj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cdnleiting.top/gtmcabciiw.html

[R26] 命令替换
来源：http://hz.cqqwz.cn/gtvrxxrgxn.html

now=$(date +%F); echo "$now"
来源：http://hz.chenjidiqi.icu/gtkfhkoxnp.html

[R27] 算术展开
来源：http://hz.yuanzhike.top/gtlqxthdcj.html

echo $((1 + 2 * 3))
来源：http://hz.zhixingplan.top/gtegftopnh.html

[R28] 浮点运算
来源：http://hz.sufxvd.cn/gthmectdgl.html

echo "scale=2; 10/3" | bc
来源：http://hz.hysaishi.cn/gtwobuyhbw.html

[R29] 定义函数
来源：http://hz.hongshengwenyu.top/gtriivoweg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hfpthk.cn/gtsbqzazjq.html

[R30] 函数返回状态码
来源：http://hz.zdqjudy.top/gtikwunafs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sysykeji.top/gtsnhoriij.html

[R31] 局部变量
来源：http://hz.quarkkingdee.top/gtmbyegyue.html

f() { local x=1; echo "$x"; }
来源：http://hz.fzhhl.top/gtohdzydqe.html

[R32] 参数个数校验
来源：http://hz.svipenyu.cn/gtkzmajolv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydjk.org.cn/gtpyjdyyzz.html

[R33] 捕获错误并提示行号
来源：http://hz.hysaishi.cn/gtupsluuxm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daxiang520.top/gtkcorymnw.html

[R34] 退出时清理
来源：http://hz.tianlin.xyz/gtdzyvncwo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtigmasigl.html

[R35] 后台执行并等待
来源：http://hz.jinghuilouyu.cn/gtccaisodg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xylfe.cn/gtndozfuua.html

[R36] 并发执行多个任务
来源：http://hz.jlsjyb.cn/gtdkcacsyi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gtyiwqyjfb.html

[R37] 把输出赋给变量
来源：http://hz.aibaodan.cn/gtfynnawul.html

files=$(ls -1)
来源：http://hz.cqqwz.cn/gtjmufkglg.html

[R38] 管道串联
来源：http://hz.yj202588.top/gtsdctptpf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hfpthk.cn/gtsnspmorg.html

[R39] 重定向标准输出与错误
来源：http://hz.yvedp.cn/gtwpwguugi.html

cmd > out.log 2>&1
来源：http://hz.zhixingplan.top/gtpqwzphxc.html

[R40] 追加写日志
来源：http://hz.haohaochexian.top/gtshlsnuvn.html

echo "log" >> out.log
来源：http://hz.nanxinkj.top/gtwjcywwhq.html

[R41] 丢弃输出
来源：http://hz.svipenyu.cn/gtgryvqmss.html

cmd >/dev/null 2>&1
来源：http://hz.yj202588.top/gtjuaylryy.html

[R42] 输入重定向
来源：http://hz.feifeiyinyue.top/gtdugarwms.html

wc -l < a.txt
来源：http://hz.tian-w.cn/gtkilgnpda.html

[R43] 按名字查找文件
来源：http://hz.daxiang520.top/gtvfxeffne.html

find . -name "*.log" -type f
来源：http://hz.yj20258888.top/gtodafrnvq.html

[R44] 按修改时间查找
来源：http://hz.yj20258.top/gtzbozpdyd.html

find . -mtime -7 -type f
来源：http://hz.yj20258888.top/gtgxjpokwk.html

[R45] 批量删除
来源：http://hz.havefunace.top/gtwlcnfcqy.html

find . -name "*.tmp" -delete
来源：http://hz.jqgufenzy.top/gtltnvgzhu.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gtfbrasplw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cucudq.cn/gtnkrbytjw.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtogcgwqxx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yanxiufei.cn/gtsnusrqzm.html

[R48] awk 取指定列
来源：http://hz.tianlin.xyz/gtmrfahmqg.html

awk '{print $1, $3}' a.txt
来源：http://hz.zdqjudy.top/gtqvwdmnsq.html

[R49] awk 带条件
来源：http://hz.hammf.cn/gtilnucwaf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yonumen.top/gtkbgxeuhb.html

[R50] awk 求和
来源：http://hz.daria6918.cn/gtpdewnnpz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hongshengwenyu.top/gtkysqvlee.html

[R51] 排序去重取前几
来源：http://hz.gaohongyu789.top/gtgzqcbsvc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jyoumei.cn/gtaxltjcke.html

[R52] 统计行数
来源：http://hz.xylfe.cn/gtotiagesg.html

wc -l a.txt
来源：http://hz.jyoumei.cn/gtruosecqk.html

[R53] 查看文件头与实时尾
来源：http://hz.tianlin.xyz/gtkteimkuw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhengqikj.top/gtalwcyfjq.html

[R54] 比较两个文件
来源：http://hz.yueranfly.top/gtxfwjeswj.html

diff a.txt b.txt
来源：http://hz.daxiang520.top/gtqmnobuds.html

[R55] 压缩与解压
来源：http://hz.zhaomingkeji.xyz/gtgaapoxdc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zdqjudy.top/gtumpxysdp.html

[R56] 远程拷贝
来源：http://hz.nanxuanxn.top/gttrssnydp.html

scp file user@host:/path/
来源：http://hz.hnxiangtu.top/gtmzxzalpe.html

[R57] 远程执行命令
来源：http://hz.xziqi.cn/gtxlkpztzr.html

ssh user@host 'uptime'
来源：http://hz.smart0.xyz/gtcxtyumni.html

[R58] 下载文件
来源：http://hz.yongpay.top/gtvdzxtvep.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pengpengdd.cyou/gtcyzgwogt.html

[R59] 发 POST JSON
来源：http://hz.cucudq.cn/gtwwfdeoxc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hammf.cn/gteghixwoj.html

[R60] 只看 HTTP 状态码
来源：http://hz.ybcxt.top/gtezwjwfho.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hnxiangtu.top/gtdzkaviet.html

[R61] 磁盘占用
来源：http://hz.tianlin.xyz/gtbkmuttkv.html

df -h;  du -sh *
来源：http://hz.yj202588.top/gtslccflel.html

[R62] 找最占空间的文件
来源：http://hz.guannengcc.top/gtdbuxyubg.html

du -ah . | sort -rh | head -10
来源：http://hz.shuidangran.top/gtnzwnqubf.html

[R63] 内存与进程
来源：http://hz.kuanghao11.cn/gtidwdcqcp.html

free -h;  ps aux | grep nginx
来源：http://hz.jinyuanbaomall.cn/gtrfbliarm.html

[R64] 结束进程
来源：http://hz.c1oappe.top/gtvnevrgsd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.bjfxy.top/gtdnhdtihx.html

[R65] 查看端口占用
来源：http://hz.jqgfzy.top/gtdsyzxnhf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhijiandao.cn/gtsrlchnzv.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtykdrggls.html

crontab -e;  crontab -l
来源：http://hz.chenlongwang.top/gtxdixeosl.html

[R67] 生成随机十六进制串
来源：http://hz.shanyushiyangkeji.top/gtffwyhifn.html

openssl rand -hex 16
来源：http://hz.smart0.xyz/gtyumksncb.html

[R68] 计算文件校验值
来源：http://hz.snrcjt.cn/gtvgpleuij.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ydzc1.top/gtavoiakuv.html

[R69] 生成随机密码
来源：http://hz.sufxvd.cn/gtnlzqayaf.html

head -c 16 /dev/urandom | base64
来源：http://hz.jiagoushi.top/gtsqojgqib.html

[R70] 时间戳与互转
来源：http://hz.xziqi.cn/gtdpybwyxh.html

date +%s;  date -d @1700000000
来源：http://hz.ppjwa.cn/gtqttnlfrh.html

[R71] 日期格式化
来源：http://hz.cucudq.cn/gtjuhnokhs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tianlin.xyz/gtmhtkojfe.html

[R72] 等待端口就绪
来源：http://hz.xziqi.cn/gtuwnymuxe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.shzxlz.cn/gtotvbfzpv.html

[R73] 分割大日志
来源：http://hz.shanyushiyangkeji.top/gtqqxmtudo.html

split -l 1000 big.log part_
来源：http://hz.hnqzz.top/gtvauqwgay.html

[R74] 批量重命名
来源：http://hz.xuanzx.com/gtmokmbfux.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pycfn.com/gteoazwoaw.html

[R75] 导出环境变量
来源：http://hz.c1oappe.top/gtcbytwrki.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhoulong.xyz/gteefsuwfg.html

[R76] 使用临时文件
来源：http://hz.snrcjt.cn/gtskalkgvt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtszfudzcu.html

[R77] 读取用户输入
来源：http://hz.shanyushiyangtech.top/gtqcwjmsnz.html

read -rp "请输入: " ans
来源：http://hz.chenjidiqi.icu/gtiytcjwfb.html

[R78] 交互式菜单
来源：http://hz.meibo888.top/gtndggjnzv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.aizwys.cn/gtamzaxrkl.html

[R79] 解析命令行选项
来源：http://hz.quarkkingdee.top/gtljonszgq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fengsongda.top/gtaevokqfn.html

[R80] 查看脚本执行耗时
来源：http://hz.gzhubu.top/gttxltutsx.html

time ./run.sh
来源：http://hz.ydzc1.top/gtjlfbbarf.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtddgpyoaz.html

S. C / C++ 专题
来源：http://hz.hywenlv.cn/gtajvoxfmo.html

================================================================================
来源：http://hz.sysykeji.top/gtbuyovvnv.html

[S01] C：Hello World
来源：http://hz.cashguo.top/gtwmsrsylf.html

#include <stdio.h>
来源：http://hz.316326.xyz/gtpqfeangv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yueranfly.top/gtwsgbabgb.html

[S02] C：变量与格式化输出
来源：http://hz.hammf.cn/gtbaeewmcv.html

int a = 10; printf("%d\n", a);
来源：http://hz.cucudq.cn/gtjlrmvhpi.html

[S03] C：读入整数
来源：http://hz.nwbrower.top/gtvrcqitwg.html

int x; scanf("%d", &x);
来源：http://hz.aizwys.cn/gtsjgmhocf.html

[S04] C：字符串复制
来源：http://hz.yj202588.top/gtdzfrxcyt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj202588.top/gtqmyxhvgy.html

[S05] C：字符串长度
来源：http://hz.xuanzx.com/gtzczhqnuo.html

strlen(s)
来源：http://hz.jiagoushi.top/gtzexxrfch.html

[S06] C：字符串比较
来源：http://hz.yongpay.top/gtyasaevub.html

strcmp(a, b) == 0
来源：http://hz.ppjwa.cn/gtubklbkms.html

[S07] C：数组遍历求和
来源：http://hz.aizwys.cn/gtyqkjdhbg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxinkj.top/gteiuqekdb.html

[S08] C：动态内存分配与释放
来源：http://hz.daxiang520.top/gtfndhbdfb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ivvv.top/gtmcnpbajj.html

[S09] C：结构体定义与初始化
来源：http://hz.ehwqpu.com/gtwzyduxtb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydjk.org.cn/gtyiqweysm.html

[S10] C：指针与解引用
来源：http://hz.snrcjt.cn/gtetwlvwku.html

int *p = &a;  *p = 5;
来源：http://hz.9152youxi.cn/gtkscmwhva.html

[S11] C：逐行读文件
来源：http://hz.gotoacloud.top/gtuzcedjyd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gaohongyu789.top/gtyrayhlwm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.wangshuangyany.cn/gtorftnmps.html

fclose(f);
来源：http://hz.nwbrower.top/gtsgpxulrb.html

[S12] C：写文件
来源：http://hz.yj20258.top/gtusqoffwl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258888.top/gttbuugwxf.html

[S13] C：宏定义
来源：http://hz.cheryme.top/gtlnhapwba.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yueranfly.top/gthixrfkst.html

[S14] C：枚举
来源：http://hz.vqdsnc.cn/gthbmszfaa.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hammf.cn/gtoxfvwyxx.html

[S15] C：类型转换
来源：http://hz.nanxinkj.top/gtajlqosoq.html

(double) a / b
来源：http://hz.bjfxy.top/gtnptqnazi.html

[S16] C：位操作置位
来源：http://hz.shuidangran.top/gtcvchibnp.html

x |= (1 << 3);
来源：http://hz.hnqzz.top/gtinavtekm.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangtech.top/gtdvwqpcdo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hywenlv.cn/gtjqocvits.html

[S18] C：命令行参数
来源：http://hz.shangyingyoupin.top/gtijremdsy.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gtadpxdgrp.html

[S19] C：快速排序
来源：http://hz.sweek.top/gtxpthgzvh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shuidangran.top/gtbyynrgme.html

[S20] C：二分查找
来源：http://hz.jinyuanbaomall.cn/gtmzumarbw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtdinxqolt.html

[S21] C：字符类别判断
来源：http://hz.zhongyouzk.top/gtanvxblge.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.kuanghao11.cn/gtcphfvkup.html

[S22] C：字符串转数字
来源：http://hz.guannengcc.top/gttapovjfc.html


<!-- 参考信息 -->