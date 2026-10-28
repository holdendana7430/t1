代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.gaohongyu789.top/gtbpasxsmp.html

[Q52] 删除指定行
来源：http://hz.fzhhl.top/gtzezrfbdg.html

DELETE FROM users WHERE id = 10;
来源：http://hz.guannengcc.top/gtssccaigo.html

[Q53] 按条件删除
来源：http://hz.yueranfly.top/gtojgbzhxs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cdnleiting.top/gteryvqfnw.html

[Q54] 清空表
来源：http://hz.snrcjt.cn/gtabcwepfn.html

TRUNCATE TABLE logs;
来源：http://hz.jinqigfzy.top/gtzglxrwdz.html

[Q55] 排名（并列占位）
来源：http://hz.hongshengwenyu.top/gtkipxlukg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.gotoacloud.top/gtwzobdjdb.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ivvv.top/gtyxawgdqc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.bjfxy.top/gthubbxpco.html

[Q57] 行号
来源：http://hz.ywan-chungtsiang.top/gtzgwaznfo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhijiandao.cn/gtxddokpdj.html

[Q58] 累计求和
来源：http://hz.jinghuilouyu.cn/gtimblbbxy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.redwolf501.top/gtoaelmibw.html

[Q59] 分组内累计
来源：http://hz.cdnleiting.top/gtkovscrdv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.hysaishi.cn/gtmsyjwlfx.html

[Q60] 取上一行 / 下一行
来源：http://hz.zycfv.cn/gtduhbqgdv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.sufxvd.cn/gtzyjwaxrr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gzhubu.top/gtyikrrvbf.html

[Q61] 移动平均
来源：http://hz.guannengcc.top/gtwidefmaa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.c1oappe.top/gtegtlbeen.html

[Q62] 分组占比
来源：http://hz.yj20258888.top/gtjlzfrcun.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.vqdsnc.cn/gtwkfiiydo.html

[Q63] 开启事务
来源：http://hz.haohaochexian.top/gtyxkyjvih.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.shuidangran.top/gtvbkrfynm.html

[Q64] 提交事务
来源：http://hz.shanyushiyangtech.top/gtylpurbex.html

COMMIT;
来源：http://hz.tianlin.xyz/gtzqtrngso.html

[Q65] 回滚事务
来源：http://hz.dashuyun.cn/gtyppbomlr.html

ROLLBACK;
来源：http://hz.fzhhl.top/gtlfmktmzv.html

[Q66] 行锁查询
来源：http://hz.yongpay.top/gtlcxwqbxy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.iojbl.cn/gthvwssxfk.html

[Q67] 设置隔离级别
来源：http://hz.jqgufenzy.top/gtztiqfvor.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.aibaodan.cn/gtpvidoxar.html

[Q68] 保存点
来源：http://hz.yj20258888.top/gtdbschmfo.html

SAVEPOINT sp1;
来源：http://hz.aibaodan.cn/gtgpfxtxcy.html

ROLLBACK TO sp1;
来源：http://hz.havefunace.top/gtsaivvgwx.html

[Q69] 查看执行计划
来源：http://hz.bjfxy.top/gtgqnorxug.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.feifeiyinyue.top/gtmdgangsn.html

[Q70] 更新统计信息
来源：http://hz.hnqzz.top/gtycbbjigq.html

ANALYZE TABLE users;
来源：http://hz.nanxuanxn.top/gtahrueyxt.html

[Q71] 查看建表语句
来源：http://hz.fzhhl.top/gtxdcbluam.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.svipenyu.cn/gtezapbqha.html

[Q72] 查看索引
来源：http://hz.cdnleiting.top/gtsbubugtt.html

SHOW INDEX FROM users;
来源：http://hz.wangdashe.top/gtggftmbwx.html

[Q73] 查看表状态
来源：http://hz.zycfv.cn/gtmtulnwgq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.birdmap.top/gthlrvatta.html

[Q74] 强制使用索引
来源：http://hz.9152youxi.cn/gterenqeji.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zdqjudy.top/gtwrohhiyz.html

[Q75] 日期格式化
来源：http://hz.yj20258888.top/gtmtcbrbdi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.havefunace.top/gtkxqiwvut.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.haohaochexian.top/gtuvniwqqo.html

[Q76] 按天统计
来源：http://hz.cashguo.top/gtqwkmrnee.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sweek.top/gtdiycklzq.html

[Q77] 时间加减
来源：http://hz.xinyue.icu/gtqafhyuyr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ehwqpu.com/gtzlhjamrq.html

[Q78] 当前时间
来源：http://hz.chenjidiqi.icu/gtuappawro.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhaomingkeji.xyz/gtiffvliwz.html

[Q79] 字符串拼接
来源：http://hz.feifeiyinyue.top/gtlbofjmyn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ydjk.org.cn/gtxxrkrbpz.html

[Q80] 字符串截取
来源：http://hz.zhiwuduotai.top/gtntzuohhx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ywan-chungtsiang.top/gtfxlvejap.html

[Q81] 字符串替换
来源：http://hz.gogol.net.cn/gtdnxnguej.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shzxlz.cn/gtlyxoacei.html

[Q82] 字符长度与字节长度
来源：http://hz.feifeiyinyue.top/gtnhiipzyz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xziqi.cn/gtpmsujjzw.html

[Q83] 大小写转换
来源：http://hz.jiagoushi.top/gtkthcbfko.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.haohaochexian.top/gtdnvkudnc.html

[Q84] 去除首尾空格
来源：http://hz.dashuyun.cn/gtriazqgnu.html

SELECT TRIM(name) FROM users;
来源：http://hz.cucudq.cn/gtywzxyauv.html

[Q85] 数值取整
来源：http://hz.daxiang520.top/gtayiyynrh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.c1oappe.top/gthlyycrkk.html

[Q86] 读取 JSON 字段
来源：http://hz.hfpthk.cn/gtrcjnlayn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sweek.top/gtldvycpwq.html

[Q87] JSON 字段做条件
来源：http://hz.svipenyu.cn/gtxejpankl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtrqthhfqn.html

[Q88] 行转列（条件聚合）
来源：http://hz.xinyue.icu/gtnsrajhax.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zdqjudy.top/gtauabvfkz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.svipenyu.cn/gtgubejtvv.html

[Q89] 判断表是否存在
来源：http://hz.xinyue.icu/gtxohbnuvl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.shuidangran.top/gtakedvirv.html

[Q90] 生成序号列
来源：http://hz.yangfankeji.com/gtsqqfhqyc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.smart0.xyz/gtiolyglzo.html

================================================================================
来源：http://hz.shuidangran.top/gtoavgynxn.html

R. Bash 专题
来源：http://hz.tian-w.cn/gtwgaoloce.html

================================================================================
来源：http://hz.gotoacloud.top/gtxitssmjh.html

[R01] shebang 与严格模式
来源：http://hz.yj202588.top/gtyuuozpah.html

#!/usr/bin/env bash
来源：http://hz.andypj.xyz/gtyjfrkijt.html

set -euo pipefail
来源：http://hz.chenjidiqi.icu/gtyijooyrr.html

[R02] 变量赋值与使用
来源：http://hz.yj20258.top/gtkfgjhxxg.html

name="Tom"; echo "$name"
来源：http://hz.xylfe.cn/gttrpgprdn.html

[R03] 只读变量
来源：http://hz.ybcxt.top/gttllsnuhe.html

readonly PI=3.14
来源：http://hz.vqdsnc.cn/gtikeajovu.html

[R04] 位置参数
来源：http://hz.ydzc1.top/gtedtesuth.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj202588.top/gtiumyqrws.html

[R05] 参数默认值
来源：http://hz.feifeiyinyue.top/gtqetcqzxs.html

name="${1:-default}"
来源：http://hz.dashuyun.cn/gtldhnedls.html

[R06] 判断命令是否存在
来源：http://hz.zhongyouzk.top/gtxvnacimc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtkfmzyzfg.html

[R07] if 判断文件
来源：http://hz.gzhubu.top/gtmtsnitxl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.52xcode.cn/gtobkqyhco.html

[R08] 数值比较
来源：http://hz.xylfe.cn/gtifcyycki.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yangfankeji.com/gtgupuwine.html

[R09] 字符串比较
来源：http://hz.gaohongyu789.top/gtgnufbady.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhijiandao.cn/gtnidaewdf.html

[R10] 正则匹配
来源：http://hz.bjfxy.top/gttpkbiggs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shangyingyoupin.top/gtnewqbcih.html

[R11] case 多分支
来源：http://hz.daxiang520.top/gtsxfwmngf.html

case "$1" in
来源：http://hz.hfpthk.cn/gtblnhpsnn.html

start) echo "启动" ;;
来源：http://hz.ppjwa.cn/gtmaghgbyk.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gtorkmhnpd.html

*)     echo "未知命令" ;;
来源：http://hz.cdnleiting.top/gtcrnyynnu.html

esac
来源：http://hz.meibo888.top/gttfzqyhqp.html

[R12] for 遍历文件
来源：http://hz.daria6918.cn/gthhxepxap.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cqqwz.cn/gtwxuqxoob.html

[R13] for 计数循环
来源：http://hz.pengpengdd.cyou/gtyiqwrgth.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gtyqvlndmq.html

[R14] C 风格 for
来源：http://hz.guowangkeji.top/gtdnzbcqrh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shuidangran.top/gtbqwpfqeb.html

[R15] while 逐行读文件
来源：http://hz.guowangkeji.top/gtxnuvibeb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xylfe.cn/gtynbxtgzn.html

[R16] until 等待条件
来源：http://hz.shangyingyoupin.top/gtkmpbzaty.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shanyushiyangkeji.top/gtkxuixuah.html

[R17] 数组定义与取值
来源：http://hz.smart0.xyz/gtqgsnmqik.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jiagoushi.top/gtpyxmbaqb.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtuetxbddx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jlsjyb.cn/gtpoytbyqa.html

[R19] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtvyhzovhv.html

echo "${#arr[@]}"
来源：http://hz.yonumen.top/gtpscavdvr.html

[R20] 关联数组（字典）
来源：http://hz.jianghu66.top/gteciplwvd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.birdmap.top/gtugaaaqgo.html

[R21] 字符串长度
来源：http://hz.cqqwz.cn/gtdrbsvuiz.html

echo "${#s}"
来源：http://hz.iojbl.cn/gtbrfhzsxj.html

[R22] 截取子串
来源：http://hz.yongpay.top/gthjbczphq.html

echo "${s:0:5}"
来源：http://hz.kuanghao11.cn/gtsiyunxbn.html

[R23] 字符串替换
来源：http://hz.jinqigufen.top/gtbyyruycl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.svipenyu.cn/gtvzoqtdyl.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gtcasxrbqi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sxryk.cn/gtbwrfwmzd.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuetiantiany.cn/gtqomreqas.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.pengpengdd.cyou/gtgengdzda.html

[R26] 命令替换
来源：http://hz.yangfankeji.com/gtrifbqznw.html

now=$(date +%F); echo "$now"
来源：http://hz.cdnleiting.top/gtouhwqkkm.html

[R27] 算术展开
来源：http://hz.kuanghao11.cn/gthwditfzr.html

echo $((1 + 2 * 3))
来源：http://hz.shzxlz.cn/gtxhmprrez.html

[R28] 浮点运算
来源：http://hz.tianlin.xyz/gtvmtkifza.html

echo "scale=2; 10/3" | bc
来源：http://hz.cdnleiting.top/gtrtqkqooo.html

[R29] 定义函数
来源：http://hz.jinqigfzy.top/gteuuebjsg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.bjfxy.top/gtjdqijwne.html

[R30] 函数返回状态码
来源：http://hz.xziqi.cn/gttjyvofki.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenlongwang.top/gttzbicgic.html

[R31] 局部变量
来源：http://hz.pengpengdd.cyou/gtvdvxiboo.html

f() { local x=1; echo "$x"; }
来源：http://hz.9152youxi.cn/gtsdutmjdr.html

[R32] 参数个数校验
来源：http://hz.shuidangran.top/gtzbwsmdyn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangkeji.top/gtkoebjbeq.html

[R33] 捕获错误并提示行号
来源：http://hz.cashguo.top/gtmewboslw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pengpengdd.cyou/gtpxvpvpff.html

[R34] 退出时清理
来源：http://hz.zhijiandao.cn/gtmvspmlcq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtrfhmgjzo.html

[R35] 后台执行并等待
来源：http://hz.shuidangran.top/gthsurnrbw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.smart0.xyz/gtoaqhbrwd.html

[R36] 并发执行多个任务
来源：http://hz.jlsjyb.cn/gtylweyvqj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xylfe.cn/gtqpvccpwz.html

[R37] 把输出赋给变量
来源：http://hz.haohaochexian.top/gtgmrmpswt.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtjvexopii.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtknxxknrf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.c1oappe.top/gtgidxlgka.html

[R39] 重定向标准输出与错误
来源：http://hz.aibaodan.cn/gtrvygaxhb.html

cmd > out.log 2>&1
来源：http://hz.ybcxt.top/gtflezqfoo.html

[R40] 追加写日志
来源：http://hz.jinqigufen.top/gtcddcyfez.html

echo "log" >> out.log
来源：http://hz.dianchejie.cn/gtegtjmjmj.html

[R41] 丢弃输出
来源：http://hz.hnxiangtu.top/gtvlzcuxbo.html

cmd >/dev/null 2>&1
来源：http://hz.pycfn.com/gtzsnebeqi.html

[R42] 输入重定向
来源：http://hz.havefunace.top/gttwlpfwkm.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtcdvzslqj.html

[R43] 按名字查找文件
来源：http://hz.hongshengwenyu.top/gtedecsyej.html

find . -name "*.log" -type f
来源：http://hz.yongpay.top/gtwnpkuloe.html

[R44] 按修改时间查找
来源：http://hz.hysaishi.cn/gtpothsfwy.html

find . -mtime -7 -type f
来源：http://hz.yuxming.cn/gtpvumtwoq.html

[R45] 批量删除
来源：http://hz.xziqi.cn/gtoprbctil.html

find . -name "*.tmp" -delete
来源：http://hz.jlsjyb.cn/gtdtaeehsk.html

[R46] 递归替换文件内容
来源：http://hz.xuetiantiany.cn/gtjuxgzaau.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gtxtlqohrn.html

[R47] sed 单行替换
来源：http://hz.nanxinkj.top/gtpyhagukf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhiwuduotai.top/gticaxgpzx.html

[R48] awk 取指定列
来源：http://hz.redwolf501.top/gtvzegklgm.html

awk '{print $1, $3}' a.txt
来源：http://hz.daxiang520.top/gtnlwwkawy.html

[R49] awk 带条件
来源：http://hz.dianchejie.cn/gtvllxxbay.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xylfe.cn/gtaqwjgmzl.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtgbydwycc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zdqjudy.top/gtrnzvvysk.html

[R51] 排序去重取前几
来源：http://hz.feifeiyinyue.top/gtmytqtqsz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.bjfxy.top/gtxsvpniie.html

[R52] 统计行数
来源：http://hz.havefunace.top/gtlsbbphol.html

wc -l a.txt
来源：http://hz.dianchejie.cn/gthfqlejsu.html

[R53] 查看文件头与实时尾
来源：http://hz.jianghu66.top/gtgkevyrrv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtoloadnkr.html

[R54] 比较两个文件
来源：http://hz.smart0.xyz/gttudwwtlj.html

diff a.txt b.txt
来源：http://hz.smart0.xyz/gtoljrwfze.html

[R55] 压缩与解压
来源：http://hz.yanxiufei.cn/gtazpulnxj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtqqdxpbmx.html

[R56] 远程拷贝
来源：http://hz.mhx1999.top/gtijoqnazu.html

scp file user@host:/path/
来源：http://hz.gaohongyu789.top/gtvmqeypti.html

[R57] 远程执行命令
来源：http://hz.zdqjudy.top/gtexjpsldc.html

ssh user@host 'uptime'
来源：http://hz.zycfv.cn/gtfnfbdtum.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtthaaqapj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gogol.net.cn/gtwnksciyi.html

[R59] 发 POST JSON
来源：http://hz.hysaishi.cn/gtykiuxnpw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinyuanbaomall.cn/gtjcengane.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtompahnso.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pengpengdd.cyou/gtlkotfupb.html

[R61] 磁盘占用
来源：http://hz.zhiwuduotai.top/gtzqcmsgeg.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gtmiculbfp.html

[R62] 找最占空间的文件
来源：http://hz.xuetiantiany.cn/gtrnptclxn.html

du -ah . | sort -rh | head -10
来源：http://hz.andypj.xyz/gtnivjiwoe.html

[R63] 内存与进程
来源：http://hz.guannengcc.top/gtujjmdutp.html

free -h;  ps aux | grep nginx
来源：http://hz.yj202588.top/gtjzjocyrs.html

[R64] 结束进程
来源：http://hz.jlsjyb.cn/gtldfgziii.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtsiyrtxja.html

[R65] 查看端口占用
来源：http://hz.feifeiyinyue.top/gtwuxqmlfh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xinyue.icu/gtvpziebse.html

[R66] 定时任务
来源：http://hz.zhixingplan.top/gtxywruxwi.html

crontab -e;  crontab -l
来源：http://hz.mhx1999.top/gtglkeqbbs.html

[R67] 生成随机十六进制串
来源：http://hz.yonumen.top/gtmtgiafkv.html

openssl rand -hex 16
来源：http://hz.sxryk.cn/gtvdjelemp.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gtdblrmszs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.pycfn.com/gtdbyjxpzq.html

[R69] 生成随机密码
来源：http://hz.xingfuxueyuan.xyz/gtmhldrysm.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gttwfggyzl.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtktbtnwhj.html

date +%s;  date -d @1700000000
来源：http://hz.gogol.net.cn/gtyowqlzfu.html

[R71] 日期格式化
来源：http://hz.nwbrower.top/gtggwbjqak.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenjidiqi.icu/gtkoxbkjgo.html

[R72] 等待端口就绪
来源：http://hz.zdqjudy.top/gtaklxfobt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gthqukckfn.html

[R73] 分割大日志
来源：http://hz.fzhhl.top/gtopoudstv.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtvnhqyyec.html

[R74] 批量重命名
来源：http://hz.jlsjyb.cn/gtgkmuffgp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.316326.xyz/gtqytjujog.html

[R75] 导出环境变量
来源：http://hz.zdqjudy.top/gtlgnlenkc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhoulong.xyz/gtvhvjbrov.html

[R76] 使用临时文件
来源：http://hz.wangdashe.top/gtthgzvyhk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtocmlxrbj.html

[R77] 读取用户输入
来源：http://hz.sxryk.cn/gtyivndpdx.html

read -rp "请输入: " ans
来源：http://hz.snrcjt.cn/gtdsvzrdex.html

[R78] 交互式菜单
来源：http://hz.sxryk.cn/gtkolzbzue.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shangyingyoupin.top/gtkqkxgrqn.html

[R79] 解析命令行选项
来源：http://hz.hnxiangtu.top/gtdihqzmuq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhaomingkeji.xyz/gtebirywdx.html

[R80] 查看脚本执行耗时
来源：http://hz.cucudq.cn/gtshyrxexc.html

time ./run.sh
来源：http://hz.yueranfly.top/gtunahmmls.html

================================================================================
来源：http://hz.nanxuanxn.top/gtkcibsxov.html

S. C / C++ 专题
来源：http://hz.cucudq.cn/gtolcqfbay.html

================================================================================
来源：http://hz.kuanghao11.cn/gtkdgtqbou.html

[S01] C：Hello World
来源：http://hz.jinqigfzy.top/gthbffebyy.html

#include <stdio.h>
来源：http://hz.jinyuanbaomall.cn/gtehccjauk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xuetiantiany.cn/gtccbazshm.html

[S02] C：变量与格式化输出
来源：http://hz.sweek.top/gtbjhyydnr.html

int a = 10; printf("%d\n", a);
来源：http://hz.birdmap.top/gtmlvhdwmx.html

[S03] C：读入整数
来源：http://hz.yongpay.top/gtbvvdanrc.html

int x; scanf("%d", &x);
来源：http://hz.ydzc1.top/gtuytwfqhc.html

[S04] C：字符串复制
来源：http://hz.hysaishi.cn/gtcngagfjz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xylfe.cn/gtvhslayho.html

[S05] C：字符串长度
来源：http://hz.jinqigufen.top/gtboljyuvd.html

strlen(s)
来源：http://hz.fengsongda.top/gtlcgmheua.html

[S06] C：字符串比较
来源：http://hz.yangfankeji.com/gtnkbrrpgb.html

strcmp(a, b) == 0
来源：http://hz.aibaodan.cn/gtotesqbgh.html

[S07] C：数组遍历求和
来源：http://hz.nanxuanxn.top/gtjeitmhwu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.haohaochexian.top/gtonplncbr.html

[S08] C：动态内存分配与释放
来源：http://hz.dianchejie.cn/gtxxhdxylo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zycfv.cn/gtqnzxgnis.html

[S09] C：结构体定义与初始化
来源：http://hz.xuanzx.com/gttchrcrpf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.snrcjt.cn/gtmlozuwfo.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtizrangcs.html

int *p = &a;  *p = 5;
来源：http://hz.gotoacloud.top/gtjtdvgaih.html

[S11] C：逐行读文件
来源：http://hz.zhengqikj.top/gtqgmwuwiv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.smart0.xyz/gtlsemnehz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shzxlz.cn/gtcxcxkxdt.html

fclose(f);
来源：http://hz.9152youxi.cn/gttompugyq.html

[S12] C：写文件
来源：http://hz.yj20258.top/gtrfttjamk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinqigufen.top/gtnadhulwc.html

[S13] C：宏定义
来源：http://hz.snrcjt.cn/gtlrbojtch.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhongyouzk.top/gtlixppcjc.html

[S14] C：枚举
来源：http://hz.yuxming.cn/gtltntrpnd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.daria6918.cn/gtmckhhpgz.html

[S15] C：类型转换
来源：http://hz.sxryk.cn/gtydfopxrq.html

(double) a / b
来源：http://hz.birdmap.top/gtjcmkgwge.html

[S16] C：位操作置位
来源：http://hz.cucudq.cn/gtzrpegeaj.html

x |= (1 << 3);
来源：http://hz.jqgfzy.top/gtwtbsslpn.html

[S17] C：安全拼接字符串
来源：http://hz.jlsjyb.cn/gtchrlfqwg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ywan-chungtsiang.top/gtooukwmbv.html

[S18] C：命令行参数
来源：http://hz.cqqwz.cn/gthgcktrga.html

int main(int argc, char **argv)
来源：http://hz.cashguo.top/gtlgbbnxmx.html

[S19] C：快速排序
来源：http://hz.jinqigfzy.top/gtigfqmpqb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtpgvdfnzc.html

[S20] C：二分查找
来源：http://hz.tanke756.top/gtovppswmx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtgmmwnefr.html

[S21] C：字符类别判断
来源：http://hz.pengpengdd.cyou/gtxbcltazz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenjidiqi.icu/gtxqtcrlfa.html

[S22] C：字符串转数字
来源：http://hz.redwolf501.top/gtrzaaazeq.html


<!-- 参考信息 -->