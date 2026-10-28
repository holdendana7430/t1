代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ehwqpu.com/gtczriwrxn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.cheryme.top/gtaxokovpw.html

[Q47] 与平均值比较
来源：http://hz.yj202588.top/gttpzbhqux.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.gotoacloud.top/gtiqxhvvgh.html

[Q48] CTE 公用表表达式
来源：http://hz.havefunace.top/gtqnpepgji.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.jinyuanbaomall.cn/gtpvmwuoph.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aibaodan.cn/gtawgvczha.html

[Q49] 更新单行
来源：http://hz.yangfankeji.com/gtvcvnxcpg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.wangshuangyany.cn/gtfvvnmeiu.html

[Q50] 批量更新
来源：http://hz.gotoacloud.top/gtpjzplwdq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.zycfv.cn/gtvtzhiayc.html

[Q51] 用子查询更新
来源：http://hz.cashguo.top/gtoglidquv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.nanxinkj.top/gtdvzciewk.html

[Q52] 删除指定行
来源：http://hz.vqdsnc.cn/gtpgxpiyga.html

DELETE FROM users WHERE id = 10;
来源：http://hz.52xcode.cn/gtombqnzis.html

[Q53] 按条件删除
来源：http://hz.svipenyu.cn/gthmayudnt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zycfv.cn/gtnltdexvz.html

[Q54] 清空表
来源：http://hz.xingfuxueyuan.xyz/gtvnqbdlhw.html

TRUNCATE TABLE logs;
来源：http://hz.52xcode.cn/gtqdhcpjfm.html

[Q55] 排名（并列占位）
来源：http://hz.fengsongda.top/gthzglgnvj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hysaishi.cn/gtnrowxfjm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.chenjidiqi.icu/gtyjhstxld.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.vqdsnc.cn/gtocomycfu.html

[Q57] 行号
来源：http://hz.jlsjyb.cn/gtmtvexths.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.jqgufenzy.top/gtzomnrzgs.html

[Q58] 累计求和
来源：http://hz.wangdashe.top/gtzcrxfwbx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nwbrower.top/gtlziezrst.html

[Q59] 分组内累计
来源：http://hz.yvedp.cn/gtnyugxtzf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sxryk.cn/gtnljjpjli.html

[Q60] 取上一行 / 下一行
来源：http://hz.sufxvd.cn/gtgbzmbmkt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.nwbrower.top/gtplblgafx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.smart0.xyz/gtovxuwovo.html

[Q61] 移动平均
来源：http://hz.ivvv.top/gtyndwhdtj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yueranfly.top/gtqprpfuby.html

[Q62] 分组占比
来源：http://hz.pengpengdd.cyou/gthukewonl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ywan-chungtsiang.top/gtdfqjzhvd.html

[Q63] 开启事务
来源：http://hz.guannengcc.top/gtvyzktqyq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigufen.top/gtznrgdlkl.html

[Q64] 提交事务
来源：http://hz.c1oappe.top/gtuthpicrj.html

COMMIT;
来源：http://hz.zhiwuduotai.top/gtefhvxqwm.html

[Q65] 回滚事务
来源：http://hz.yuanzhike.top/gtfiahwizz.html

ROLLBACK;
来源：http://hz.aibaodan.cn/gtbzqodxho.html

[Q66] 行锁查询
来源：http://hz.yj20258888.top/gtqfpmvqxz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jianghu66.top/gteqagocir.html

[Q67] 设置隔离级别
来源：http://hz.nanxuanxn.top/gtoimtiahh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.fzhhl.top/gtchliwrjm.html

[Q68] 保存点
来源：http://hz.jqgufenzy.top/gtjfiabeqn.html

SAVEPOINT sp1;
来源：http://hz.yuanzhike.top/gtgdrlmbfc.html

ROLLBACK TO sp1;
来源：http://hz.aizwys.cn/gtbzzqwjrw.html

[Q69] 查看执行计划
来源：http://hz.havefunace.top/gtmulxwxso.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.dashuyun.cn/gtaowulqhl.html

[Q70] 更新统计信息
来源：http://hz.zhongyouzk.top/gtvmdtigfv.html

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gtnqmczxme.html

[Q71] 查看建表语句
来源：http://hz.hongshengwenyu.top/gtwokwamat.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhaomingkeji.xyz/gtgzbfgrcr.html

[Q72] 查看索引
来源：http://hz.cqqwz.cn/gtkerkpssm.html

SHOW INDEX FROM users;
来源：http://hz.ppjwa.cn/gtqrchsoys.html

[Q73] 查看表状态
来源：http://hz.iojbl.cn/gtujqbrsgt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.tian-w.cn/gtfpizryie.html

[Q74] 强制使用索引
来源：http://hz.zycfv.cn/gtokxfrpix.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gaohongyu789.top/gtdomggwzk.html

[Q75] 日期格式化
来源：http://hz.smart0.xyz/gtguwyuuqs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cashguo.top/gthnpsxmdt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.quarkkingdee.top/gtxzsywdze.html

[Q76] 按天统计
来源：http://hz.yuanzhike.top/gtryzuhymk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.zhoulong.xyz/gtpmzdlala.html

[Q77] 时间加减
来源：http://hz.aibaodan.cn/gtoxlvlkkw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.guowangkeji.top/gtzwphgqvw.html

[Q78] 当前时间
来源：http://hz.xylfe.cn/gtnpltwjnl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gogol.net.cn/gtcflsnuym.html

[Q79] 字符串拼接
来源：http://hz.gaohongyu789.top/gtnloexxtp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zdqjudy.top/gtihipooye.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtmnxifwhq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.quarkkingdee.top/gtcmvinmbe.html

[Q81] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gtmtowdbcp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nanxuanxn.top/gtucmkxmsy.html

[Q82] 字符长度与字节长度
来源：http://hz.haohaochexian.top/gttrocgotl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtxzzbkiiu.html

[Q83] 大小写转换
来源：http://hz.sxryk.cn/gtrxqslpfb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hywenlv.cn/gtrsqattjo.html

[Q84] 去除首尾空格
来源：http://hz.aibaodan.cn/gtqrvapcfq.html

SELECT TRIM(name) FROM users;
来源：http://hz.xylfe.cn/gthogymxyw.html

[Q85] 数值取整
来源：http://hz.xuetiantiany.cn/gtvarozvul.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigufen.top/gttjfirgvo.html

[Q86] 读取 JSON 字段
来源：http://hz.cucudq.cn/gtayslhkwy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yangfankeji.com/gtgeyaqmtv.html

[Q87] JSON 字段做条件
来源：http://hz.vqdsnc.cn/gtrczqasrb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.fzhhl.top/gtyofesfbj.html

[Q88] 行转列（条件聚合）
来源：http://hz.yongpay.top/gtcxqarhul.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nwbrower.top/gtskfijemv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtqhfjcidb.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtayxfxtrb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.daxiang520.top/gtouwfkxxk.html

[Q90] 生成序号列
来源：http://hz.hnxiangtu.top/gtwskxcnob.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhoulong.xyz/gtamqqgbvg.html

================================================================================
来源：http://hz.yanxiufei.cn/gtakkmettu.html

R. Bash 专题
来源：http://hz.jinghuilouyu.cn/gtwuggxifp.html

================================================================================
来源：http://hz.sufxvd.cn/gtguslxhnk.html

[R01] shebang 与严格模式
来源：http://hz.zhaomingkeji.xyz/gtzwhfmvay.html

#!/usr/bin/env bash
来源：http://hz.guannengcc.top/gtgohduxhw.html

set -euo pipefail
来源：http://hz.yongpay.top/gtangaetzp.html

[R02] 变量赋值与使用
来源：http://hz.kuanghao11.cn/gtuctlvdcw.html

name="Tom"; echo "$name"
来源：http://hz.zhijiandao.cn/gttogtkezs.html

[R03] 只读变量
来源：http://hz.svipenyu.cn/gtdqigqute.html

readonly PI=3.14
来源：http://hz.shuidangran.top/gtwvmejebq.html

[R04] 位置参数
来源：http://hz.zhixingplan.top/gtoxdtqava.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangtech.top/gtmmssvimg.html

[R05] 参数默认值
来源：http://hz.zhongyouzk.top/gtoudmmwce.html

name="${1:-default}"
来源：http://hz.bjfxy.top/gthhwgsuvx.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gtlfakaywh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.snrcjt.cn/gtbehihkfw.html

[R07] if 判断文件
来源：http://hz.ehwqpu.com/gtlmshluyt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gaohongyu789.top/gtizobwlst.html

[R08] 数值比较
来源：http://hz.xuanzx.com/gtyoufnxof.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gthjmxqxak.html

[R09] 字符串比较
来源：http://hz.smart0.xyz/gtacojgxtn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hfpthk.cn/gtnzjuvkpn.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gttmedostj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hongshengwenyu.top/gthkxfmwkp.html

[R11] case 多分支
来源：http://hz.jinyuanbaomall.cn/gtdmyhnspt.html

case "$1" in
来源：http://hz.jqgfzy.top/gtnrrnmasq.html

start) echo "启动" ;;
来源：http://hz.feifeiyinyue.top/gtlmlqcblk.html

stop)  echo "停止" ;;
来源：http://hz.nwbrower.top/gtplblasvc.html

*)     echo "未知命令" ;;
来源：http://hz.xingfuxueyuan.xyz/gtwaicvmgb.html

esac
来源：http://hz.jianghu66.top/gtjpzjglar.html

[R12] for 遍历文件
来源：http://hz.nanxuanxn.top/gtnztmdypb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.meibo888.top/gtkfhvkqlk.html

[R13] for 计数循环
来源：http://hz.ehwqpu.com/gtkjuagqct.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sxryk.cn/gtojnsobbx.html

[R14] C 风格 for
来源：http://hz.zhijiandao.cn/gtovzsumnh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtmqvhyhbm.html

[R15] while 逐行读文件
来源：http://hz.jyoumei.cn/gtuvwexpow.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cashguo.top/gtekrcnyqw.html

[R16] until 等待条件
来源：http://hz.chenjidiqi.icu/gtgatsvgzs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yvedp.cn/gtqtimxfch.html

[R17] 数组定义与取值
来源：http://hz.meibo888.top/gtrxflgnhq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xingfuxueyuan.xyz/gtzyngpzii.html

[R18] 遍历数组
来源：http://hz.hammf.cn/gttdvmwnhc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shzxlz.cn/gtscbdmbaw.html

[R19] 数组长度
来源：http://hz.zhongyouzk.top/gtiamtikma.html

echo "${#arr[@]}"
来源：http://hz.zhaomingkeji.xyz/gtyfwcmbkh.html

[R20] 关联数组（字典）
来源：http://hz.ivvv.top/gtgjpotpkl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cucudq.cn/gtwkchcmsd.html

[R21] 字符串长度
来源：http://hz.wangshuangyany.cn/gtaimxrord.html

echo "${#s}"
来源：http://hz.zhiwuduotai.top/gtqimmysgz.html

[R22] 截取子串
来源：http://hz.havefunace.top/gtorsnoxri.html

echo "${s:0:5}"
来源：http://hz.cashguo.top/gtljlsevkq.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtfpbtkxqc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.guannengcc.top/gtucivoijg.html

[R24] 大小写转换
来源：http://hz.daxiang520.top/gtelsfoiol.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tianlin.xyz/gtqpsvrffp.html

[R25] 去后缀 / 去前缀
来源：http://hz.yangfankeji.com/gtzjwwwday.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.havefunace.top/gtbepcrkuc.html

[R26] 命令替换
来源：http://hz.dashuyun.cn/gtrwxjizqo.html

now=$(date +%F); echo "$now"
来源：http://hz.pengpengdd.cyou/gtoahrnzoi.html

[R27] 算术展开
来源：http://hz.jinqigufen.top/gtqjdoxkzx.html

echo $((1 + 2 * 3))
来源：http://hz.cheryme.top/gthevjeowd.html

[R28] 浮点运算
来源：http://hz.cqqwz.cn/gtpszhlnqr.html

echo "scale=2; 10/3" | bc
来源：http://hz.guannengcc.top/gtvtkbiine.html

[R29] 定义函数
来源：http://hz.daxiang520.top/gtacfsgcxc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jlsjyb.cn/gtkkxptpoy.html

[R30] 函数返回状态码
来源：http://hz.zhixingplan.top/gtpvgmyegu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenlongwang.top/gtdqojoxxb.html

[R31] 局部变量
来源：http://hz.nanxinkj.top/gtnbgvnhrm.html

f() { local x=1; echo "$x"; }
来源：http://hz.jlsjyb.cn/gtmytszqsx.html

[R32] 参数个数校验
来源：http://hz.gotoacloud.top/gtyjosvvvu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ehwqpu.com/gtyonykzfl.html

[R33] 捕获错误并提示行号
来源：http://hz.jinyuanbaomall.cn/gtbmlbsrri.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuetiantiany.cn/gttkhvizor.html

[R34] 退出时清理
来源：http://hz.gotoacloud.top/gtwxhxehqs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtbwodhkbq.html

[R35] 后台执行并等待
来源：http://hz.hnxiangtu.top/gtldkoamti.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ywan-chungtsiang.top/gtudegcpoq.html

[R36] 并发执行多个任务
来源：http://hz.52xcode.cn/gttlrtrwmu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pengpengdd.cyou/gtfhhlztfl.html

[R37] 把输出赋给变量
来源：http://hz.feifeiyinyue.top/gtkbroeeox.html

files=$(ls -1)
来源：http://hz.zhaomingkeji.xyz/gtrmkbgqkj.html

[R38] 管道串联
来源：http://hz.316326.xyz/gtebuievlf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.wangdashe.top/gtskgztmmq.html

[R39] 重定向标准输出与错误
来源：http://hz.shzxlz.cn/gtplwwylbx.html

cmd > out.log 2>&1
来源：http://hz.sufxvd.cn/gtxkayqkqy.html

[R40] 追加写日志
来源：http://hz.xuanzx.com/gtswguhszi.html

echo "log" >> out.log
来源：http://hz.jinghuilouyu.cn/gtzmnvvwea.html

[R41] 丢弃输出
来源：http://hz.cashguo.top/gtkukhdsxy.html

cmd >/dev/null 2>&1
来源：http://hz.haohaochexian.top/gtehirzmwm.html

[R42] 输入重定向
来源：http://hz.yanxiufei.cn/gtuylqzbbr.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtwmskcxgt.html

[R43] 按名字查找文件
来源：http://hz.hywenlv.cn/gtrpafpsci.html

find . -name "*.log" -type f
来源：http://hz.chenzaomai.com/gtxkmzefhn.html

[R44] 按修改时间查找
来源：http://hz.zhijiandao.cn/gtywroflhr.html

find . -mtime -7 -type f
来源：http://hz.zhengqikj.top/gteualczfh.html

[R45] 批量删除
来源：http://hz.hongshengwenyu.top/gtvlgbrxnn.html

find . -name "*.tmp" -delete
来源：http://hz.jinyuanbaomall.cn/gtmzfprypr.html

[R46] 递归替换文件内容
来源：http://hz.jqgufenzy.top/gteaecnhdb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.iojbl.cn/gtbpzrbbvo.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gtavmbqkvo.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangdashe.top/gtkccetbpd.html

[R48] awk 取指定列
来源：http://hz.52xcode.cn/gthjnsepwk.html

awk '{print $1, $3}' a.txt
来源：http://hz.9152youxi.cn/gtgbnstrkr.html

[R49] awk 带条件
来源：http://hz.wangdashe.top/gtiggwzjpe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hfpthk.cn/gtttflqgzy.html

[R50] awk 求和
来源：http://hz.kuanghao11.cn/gthxcllelq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.kuanghao11.cn/gtozdfhyrv.html

[R51] 排序去重取前几
来源：http://hz.yj202588.top/gtuhypxqqd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.smart0.xyz/gtieymtxtg.html

[R52] 统计行数
来源：http://hz.jinqigufen.top/gtjyoctbih.html

wc -l a.txt
来源：http://hz.shangyingyoupin.top/gtxiplwepe.html

[R53] 查看文件头与实时尾
来源：http://hz.jyoumei.cn/gtbhplxxni.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gteoxcpcwm.html

[R54] 比较两个文件
来源：http://hz.tian-w.cn/gtcouqfqod.html

diff a.txt b.txt
来源：http://hz.52xcode.cn/gtsndjrrjh.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangtech.top/gtgxudxobo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.tianlin.xyz/gtevyddedy.html

[R56] 远程拷贝
来源：http://hz.hfpthk.cn/gtuwsxxaxj.html

scp file user@host:/path/
来源：http://hz.daria6918.cn/gtebgxqowv.html

[R57] 远程执行命令
来源：http://hz.daria6918.cn/gturxofkcp.html

ssh user@host 'uptime'
来源：http://hz.gogol.net.cn/gtpnqkeqcy.html

[R58] 下载文件
来源：http://hz.kuanghao11.cn/gtsnlhapfw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hongshengwenyu.top/gthidcwres.html

[R59] 发 POST JSON
来源：http://hz.chenlongwang.top/gtrhtlhcvj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.iojbl.cn/gthufgakrk.html

[R60] 只看 HTTP 状态码
来源：http://hz.hysaishi.cn/gtbfwvmakp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zycfv.cn/gtzrlkcswo.html

[R61] 磁盘占用
来源：http://hz.ydzc1.top/gtwagquwfa.html

df -h;  du -sh *
来源：http://hz.hnqzz.top/gtqgvwbhax.html

[R62] 找最占空间的文件
来源：http://hz.zhoulong.xyz/gtituzwevg.html

du -ah . | sort -rh | head -10
来源：http://hz.xuetiantiany.cn/gtuqryxgzv.html

[R63] 内存与进程
来源：http://hz.yvedp.cn/gtklnvovng.html

free -h;  ps aux | grep nginx
来源：http://hz.316326.xyz/gtxyvrvgtw.html

[R64] 结束进程
来源：http://hz.nanxuanxn.top/gtwxsiwftu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shuidangran.top/gtvyglrdvp.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtcclhlnic.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xylfe.cn/gtsqrykvlv.html

[R66] 定时任务
来源：http://hz.sxryk.cn/gtgmelbcof.html

crontab -e;  crontab -l
来源：http://hz.zhixingplan.top/gtfacgqdqi.html

[R67] 生成随机十六进制串
来源：http://hz.hysaishi.cn/gtyvbxmlil.html

openssl rand -hex 16
来源：http://hz.feifeiyinyue.top/gtvdohxggi.html

[R68] 计算文件校验值
来源：http://hz.fzhhl.top/gtukwjtqxa.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hnqzz.top/gtyhnprqqz.html

[R69] 生成随机密码
来源：http://hz.jiagoushi.top/gtmbjmppbz.html

head -c 16 /dev/urandom | base64
来源：http://hz.vqdsnc.cn/gtxnzaeagl.html

[R70] 时间戳与互转
来源：http://hz.ydzc1.top/gtaxzxfwic.html

date +%s;  date -d @1700000000
来源：http://hz.zhongyouzk.top/gtewayphzt.html

[R71] 日期格式化
来源：http://hz.jinqigfzy.top/gtyqluhaiw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hongshengwenyu.top/gtqhpejrpv.html

[R72] 等待端口就绪
来源：http://hz.ivvv.top/gtkgghbekk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.svipenyu.cn/gtzyccomif.html

[R73] 分割大日志
来源：http://hz.yvedp.cn/gthzrulxnd.html

split -l 1000 big.log part_
来源：http://hz.yj20258.top/gtujsyjcec.html

[R74] 批量重命名
来源：http://hz.gaohongyu789.top/gttcawbklu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pycfn.com/gtqscxdmpy.html

[R75] 导出环境变量
来源：http://hz.daxiang520.top/gtjshbbkxi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.andypj.xyz/gtkuloimhc.html

[R76] 使用临时文件
来源：http://hz.zycfv.cn/gtkoojfzjz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtzhflvovp.html

[R77] 读取用户输入
来源：http://hz.gotoacloud.top/gtlsckicae.html

read -rp "请输入: " ans
来源：http://hz.jlsjyb.cn/gtzbucmdjm.html

[R78] 交互式菜单
来源：http://hz.jinghuilouyu.cn/gtahjxyodl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sufxvd.cn/gtoyrotpan.html

[R79] 解析命令行选项
来源：http://hz.bjfxy.top/gtjpxeleqv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sufxvd.cn/gtjhirphyv.html

[R80] 查看脚本执行耗时
来源：http://hz.gotoacloud.top/gthyijlsoa.html

time ./run.sh
来源：http://hz.guannengcc.top/gtnamivonm.html

================================================================================
来源：http://hz.wangdashe.top/gtnqfjpqqc.html

S. C / C++ 专题
来源：http://hz.yueranfly.top/gtfyqilsro.html

================================================================================
来源：http://hz.svipenyu.cn/gtgehmfjci.html

[S01] C：Hello World
来源：http://hz.nwbrower.top/gtvkceuxmm.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtvgdmvtir.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.birdmap.top/gtedlhkxnf.html

[S02] C：变量与格式化输出
来源：http://hz.jyoumei.cn/gtrhtruhza.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhijiandao.cn/gtvwrkoujp.html

[S03] C：读入整数
来源：http://hz.feifeiyinyue.top/gthpogqrcs.html

int x; scanf("%d", &x);
来源：http://hz.quarkkingdee.top/gtzuryadql.html

[S04] C：字符串复制
来源：http://hz.andypj.xyz/gtrnestxcx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.birdmap.top/gtuiqndwvg.html

[S05] C：字符串长度
来源：http://hz.sysykeji.top/gthirpanaz.html

strlen(s)
来源：http://hz.yuxming.cn/gtwfhoekae.html

[S06] C：字符串比较
来源：http://hz.shangyingyoupin.top/gttbauqzpt.html

strcmp(a, b) == 0
来源：http://hz.dashuyun.cn/gteaynvzoj.html

[S07] C：数组遍历求和
来源：http://hz.kuanghao11.cn/gtxgrkaopk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xinyue.icu/gtyoriwysu.html

[S08] C：动态内存分配与释放
来源：http://hz.ehwqpu.com/gtpmavvzpq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cheryme.top/gtufgbjtme.html

[S09] C：结构体定义与初始化
来源：http://hz.ydjk.org.cn/gtyuqlrsfk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuanzhike.top/gtqfzpqyec.html

[S10] C：指针与解引用
来源：http://hz.wangshuangyany.cn/gtknkqofct.html

int *p = &a;  *p = 5;
来源：http://hz.ydjk.org.cn/gtxqgqaulx.html

[S11] C：逐行读文件
来源：http://hz.aibaodan.cn/gtnuiacgqa.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hammf.cn/gtyntqwweo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ehwqpu.com/gtbdivzwkk.html

fclose(f);
来源：http://hz.gogol.net.cn/gtsvhhavoo.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtjcrdcrta.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.meibo888.top/gtccdiszwa.html

[S13] C：宏定义
来源：http://hz.shanyushiyangtech.top/gtkahhivjm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gtghluivrn.html

[S14] C：枚举
来源：http://hz.ydjk.org.cn/gtuabjxyxw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgfzy.top/gtvuipsvqy.html

[S15] C：类型转换
来源：http://hz.smart0.xyz/gtcttgpfhb.html

(double) a / b
来源：http://hz.zdqjudy.top/gtyjjwbzss.html

[S16] C：位操作置位
来源：http://hz.daxiang520.top/gtozyyrgod.html


<!-- 参考信息 -->