代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hz.iojbl.cn/gtextgibjt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ydzc1.top/gtcfoabznm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.yj202588.top/gtrrvbtmyq.html

[Q49] 更新单行
来源：http://hz.hfpthk.cn/gtzfaocxzq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.c1oappe.top/gteoovkrjb.html

[Q50] 批量更新
来源：http://hz.meibo888.top/gtahgfrpzp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sysykeji.top/gtiyqbcirp.html

[Q51] 用子查询更新
来源：http://hz.52xcode.cn/gtcgidvfyq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.hnqzz.top/gtrvilbfvw.html

[Q52] 删除指定行
来源：http://hz.pengpengdd.cyou/gtjuenklpv.html

DELETE FROM users WHERE id = 10;
来源：http://hz.xuanzx.com/gtwspkfaon.html

[Q53] 按条件删除
来源：http://hz.wangshuangyany.cn/gtxnlbrjgc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shangyingyoupin.top/gtoezmhpfn.html

[Q54] 清空表
来源：http://hz.hywenlv.cn/gtvyzhtlpy.html

TRUNCATE TABLE logs;
来源：http://hz.shanyushiyangkeji.top/gtcwzxfeqj.html

[Q55] 排名（并列占位）
来源：http://hz.xinyue.icu/gtvnxmlqdi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ehwqpu.com/gtpihotsjm.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtghliwdai.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nanxinkj.top/gtyyncfvpf.html

[Q57] 行号
来源：http://hz.hywenlv.cn/gtyhccdojk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hammf.cn/gtokjrzpdi.html

[Q58] 累计求和
来源：http://hz.ywan-chungtsiang.top/gtkmzijrux.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.wangshuangyany.cn/gtxwknhgej.html

[Q59] 分组内累计
来源：http://hz.fzhhl.top/gtozduujmw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guannengcc.top/gtpwmyoiao.html

[Q60] 取上一行 / 下一行
来源：http://hz.hysaishi.cn/gtklmmcgnw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhiwuduotai.top/gtkyhgwzvb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.c1oappe.top/gthyoqowub.html

[Q61] 移动平均
来源：http://hz.smart0.xyz/gtarswetdv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yangfankeji.com/gtzldwnzhn.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtqbrezvpn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jianghu66.top/gtoasckpul.html

[Q63] 开启事务
来源：http://hz.shangyingyoupin.top/gtlpkuuugb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yueranfly.top/gtkejoptxq.html

[Q64] 提交事务
来源：http://hz.meibo888.top/gtkbaouwxy.html

COMMIT;
来源：http://hz.hnqzz.top/gtafsapreb.html

[Q65] 回滚事务
来源：http://hz.xziqi.cn/gtfdhteime.html

ROLLBACK;
来源：http://hz.daxiang520.top/gtxamdwyku.html

[Q66] 行锁查询
来源：http://hz.jinghuilouyu.cn/gtemgfaxgi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.cheryme.top/gtfqllajro.html

[Q67] 设置隔离级别
来源：http://hz.nanxinkj.top/gtafzexjkx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.jqgfzy.top/gtnugbaufi.html

[Q68] 保存点
来源：http://hz.ydzc1.top/gtiztfrxrj.html

SAVEPOINT sp1;
来源：http://hz.ydzc1.top/gtclfnkine.html

ROLLBACK TO sp1;
来源：http://hz.yvedp.cn/gtbrbvxesj.html

[Q69] 查看执行计划
来源：http://hz.yonumen.top/gtydpoeeld.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.mhx1999.top/gtwndjvakc.html

[Q70] 更新统计信息
来源：http://hz.52xcode.cn/gtvbifxkzd.html

ANALYZE TABLE users;
来源：http://hz.jinghuilouyu.cn/gtilkwwvmj.html

[Q71] 查看建表语句
来源：http://hz.sweek.top/gtuekmlbpf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhaomingkeji.xyz/gtlxeppvbn.html

[Q72] 查看索引
来源：http://hz.xylfe.cn/gtikvsejxq.html

SHOW INDEX FROM users;
来源：http://hz.tanke756.top/gtakpmapnz.html

[Q73] 查看表状态
来源：http://hz.chenzaomai.com/gtizsmpxft.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.andypj.xyz/gtqnnfhdid.html

[Q74] 强制使用索引
来源：http://hz.hammf.cn/gtyxftpxfb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.svipenyu.cn/gtmchrgyfe.html

[Q75] 日期格式化
来源：http://hz.hywenlv.cn/gtxhlpuafg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cdnleiting.top/gtjubdhhjp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xinyue.icu/gtcsjxfbka.html

[Q76] 按天统计
来源：http://hz.zdqjudy.top/gtyrokciva.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ivvv.top/gtdmcbhpgu.html

[Q77] 时间加减
来源：http://hz.quarkkingdee.top/gtnhinieez.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hysaishi.cn/gtuusysuyr.html

[Q78] 当前时间
来源：http://hz.nwbrower.top/gtgariqgvl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinqigufen.top/gtkqbgtufy.html

[Q79] 字符串拼接
来源：http://hz.iojbl.cn/gtpmqkrrho.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhaomingkeji.xyz/gthmzndcyf.html

[Q80] 字符串截取
来源：http://hz.cdnleiting.top/gtbvekofll.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ehwqpu.com/gtrbrjqwlx.html

[Q81] 字符串替换
来源：http://hz.c1oappe.top/gtfdbevfzy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.daxiang520.top/gtdrkrrdmm.html

[Q82] 字符长度与字节长度
来源：http://hz.ivvv.top/gtjypyvvck.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hammf.cn/gtbgknvwmo.html

[Q83] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtotvrhvda.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jqgfzy.top/gtkglwmrqf.html

[Q84] 去除首尾空格
来源：http://hz.kuanghao11.cn/gthiaztnig.html

SELECT TRIM(name) FROM users;
来源：http://hz.jyoumei.cn/gtecpcvcew.html

[Q85] 数值取整
来源：http://hz.pycfn.com/gtinqudyiu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xuanzx.com/gtofodhxax.html

[Q86] 读取 JSON 字段
来源：http://hz.tianlin.xyz/gteppknddh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gogol.net.cn/gtfmcyiovg.html

[Q87] JSON 字段做条件
来源：http://hz.daxiang520.top/gtizursibu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.c1oappe.top/gtrktnwkwq.html

[Q88] 行转列（条件聚合）
来源：http://hz.yongpay.top/gtuggwcrlb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigufen.top/gtdsnrbeug.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydzc1.top/gtlozfaiex.html

[Q89] 判断表是否存在
来源：http://hz.ppjwa.cn/gtqdvplkpl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ywan-chungtsiang.top/gtlznoqizh.html

[Q90] 生成序号列
来源：http://hz.nanxinkj.top/gtoxbokdgo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.cheryme.top/gtqynpsniu.html

================================================================================
来源：http://hz.pycfn.com/gtjaqomlfg.html

R. Bash 专题
来源：http://hz.ywan-chungtsiang.top/gtldblfvuu.html

================================================================================
来源：http://hz.jiagoushi.top/gtmvcaczsd.html

[R01] shebang 与严格模式
来源：http://hz.jianghu66.top/gtmkkdzxyd.html

#!/usr/bin/env bash
来源：http://hz.xuetiantiany.cn/gttzhtisvj.html

set -euo pipefail
来源：http://hz.fengsongda.top/gtqzquasab.html

[R02] 变量赋值与使用
来源：http://hz.kuanghao11.cn/gtcqbhtvug.html

name="Tom"; echo "$name"
来源：http://hz.daxiang520.top/gtcmkxdwiw.html

[R03] 只读变量
来源：http://hz.zhengqikj.top/gtsuncrhqz.html

readonly PI=3.14
来源：http://hz.yuanzhike.top/gtrbwjnmfw.html

[R04] 位置参数
来源：http://hz.yuanzhike.top/gtkcsfzmud.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xinyue.icu/gtwzyrxgqs.html

[R05] 参数默认值
来源：http://hz.hysaishi.cn/gtrmappuzb.html

name="${1:-default}"
来源：http://hz.hywenlv.cn/gtpyncglhx.html

[R06] 判断命令是否存在
来源：http://hz.xingfuxueyuan.xyz/gtcgqendeb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shuidangran.top/gtrqaczvyt.html

[R07] if 判断文件
来源：http://hz.xingfuxueyuan.xyz/gtaqtijovn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guowangkeji.top/gtpdcmkqjn.html

[R08] 数值比较
来源：http://hz.nwbrower.top/gtgfttpytg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.quarkkingdee.top/gthukddrzy.html

[R09] 字符串比较
来源：http://hz.ppjwa.cn/gtoaixkgbl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhijiandao.cn/gtqodnolxv.html

[R10] 正则匹配
来源：http://hz.zhixingplan.top/gtnpdsuwuk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tanke756.top/gtdcyhmlct.html

[R11] case 多分支
来源：http://hz.hywenlv.cn/gtmcmziqrr.html

case "$1" in
来源：http://hz.hongshengwenyu.top/gttqilnbnm.html

start) echo "启动" ;;
来源：http://hz.yanxiufei.cn/gtyqutqtbm.html

stop)  echo "停止" ;;
来源：http://hz.guowangkeji.top/gtnweagike.html

*)     echo "未知命令" ;;
来源：http://hz.fengsongda.top/gtcrhcmrod.html

esac
来源：http://hz.sweek.top/gtkvkcuigy.html

[R12] for 遍历文件
来源：http://hz.zhiwuduotai.top/gtvupojijm.html

for f in *.txt; do echo "$f"; done
来源：http://hz.c1oappe.top/gtfmmmffet.html

[R13] for 计数循环
来源：http://hz.shanyushiyangtech.top/gtlcpebrcw.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.shanyushiyangtech.top/gtwlbczhsn.html

[R14] C 风格 for
来源：http://hz.wangdashe.top/gthlicxmwq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gzhubu.top/gtviqxmwjo.html

[R15] while 逐行读文件
来源：http://hz.sxryk.cn/gtpbinvtzv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.feifeiyinyue.top/gtuxlhrzlt.html

[R16] until 等待条件
来源：http://hz.tian-w.cn/gtwpgwhbok.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zdqjudy.top/gtfcylduox.html

[R17] 数组定义与取值
来源：http://hz.jinqigfzy.top/gtiecwdljn.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shzxlz.cn/gtbnozypxx.html

[R18] 遍历数组
来源：http://hz.kuanghao11.cn/gtdrctiwxt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuanzx.com/gtlrrjcyzv.html

[R19] 数组长度
来源：http://hz.sweek.top/gtuvdsxxal.html

echo "${#arr[@]}"
来源：http://hz.dianchejie.cn/gtglzdysgh.html

[R20] 关联数组（字典）
来源：http://hz.cucudq.cn/gtdsmffbeg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.daxiang520.top/gtxoeajcbk.html

[R21] 字符串长度
来源：http://hz.hnxiangtu.top/gtbnrkovoc.html

echo "${#s}"
来源：http://hz.ydjk.org.cn/gtsbibkqib.html

[R22] 截取子串
来源：http://hz.jinghuilouyu.cn/gtngfwlerw.html

echo "${s:0:5}"
来源：http://hz.jinghuilouyu.cn/gtjeekvydx.html

[R23] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gtdzwrkqjj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtfijgnqrj.html

[R24] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtwmooxfch.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ivvv.top/gtulwfvzfm.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtpuvgrgsx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.0kj1m.cn/gtreavnukr.html

[R26] 命令替换
来源：http://hz.yvedp.cn/gtexzbuxhv.html

now=$(date +%F); echo "$now"
来源：http://hz.ivvv.top/gtprsesavt.html

[R27] 算术展开
来源：http://hz.fengsongda.top/gtodiouith.html

echo $((1 + 2 * 3))
来源：http://hz.fengsongda.top/gtcuinawqe.html

[R28] 浮点运算
来源：http://hz.gogol.net.cn/gtlgrrevdd.html

echo "scale=2; 10/3" | bc
来源：http://hz.yueranfly.top/gtjtfvgvql.html

[R29] 定义函数
来源：http://hz.gzhubu.top/gtuqtrhizr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgufenzy.top/gtjlgesrib.html

[R30] 函数返回状态码
来源：http://hz.zdqjudy.top/gtreowuitj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtxyxvrton.html

[R31] 局部变量
来源：http://hz.haohaochexian.top/gtdiptljbz.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenlongwang.top/gtrxsmcdcc.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtislmcqdw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtnbzwjuwp.html

[R33] 捕获错误并提示行号
来源：http://hz.chenjidiqi.icu/gtbugbrhtk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cheryme.top/gtrcdrizch.html

[R34] 退出时清理
来源：http://hz.gotoacloud.top/gtarhcjjhs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.shuidangran.top/gtkasoivzo.html

[R35] 后台执行并等待
来源：http://hz.cqqwz.cn/gtfqrmpjfe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sweek.top/gtnlfyewib.html

[R36] 并发执行多个任务
来源：http://hz.ydzc1.top/gtsrylyzjr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gaohongyu789.top/gtaecbfmft.html

[R37] 把输出赋给变量
来源：http://hz.iojbl.cn/gtvibhzoyy.html

files=$(ls -1)
来源：http://hz.0kj1m.cn/gtkarbxyze.html

[R38] 管道串联
来源：http://hz.jinyuanbaomall.cn/gtdmbdzwlx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yueranfly.top/gtllufbfwf.html

[R39] 重定向标准输出与错误
来源：http://hz.sweek.top/gttazqwvnn.html

cmd > out.log 2>&1
来源：http://hz.fzhhl.top/gtracobjju.html

[R40] 追加写日志
来源：http://hz.guannengcc.top/gtvapdqlxy.html

echo "log" >> out.log
来源：http://hz.shuidangran.top/gtttwlfbks.html

[R41] 丢弃输出
来源：http://hz.shanyushiyangkeji.top/gtmiavdamx.html

cmd >/dev/null 2>&1
来源：http://hz.tian-w.cn/gtgemoiulr.html

[R42] 输入重定向
来源：http://hz.shzxlz.cn/gthyxkongm.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gtuwjqiybg.html

[R43] 按名字查找文件
来源：http://hz.fzhhl.top/gtjxrzlabh.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangtech.top/gteqmoyjtt.html

[R44] 按修改时间查找
来源：http://hz.yonumen.top/gtxrpfvfsf.html

find . -mtime -7 -type f
来源：http://hz.svipenyu.cn/gtqeluyrzk.html

[R45] 批量删除
来源：http://hz.cheryme.top/gtdmlhcafg.html

find . -name "*.tmp" -delete
来源：http://hz.hnxiangtu.top/gtfkecbayn.html

[R46] 递归替换文件内容
来源：http://hz.9152youxi.cn/gtidkhmfot.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nwbrower.top/gtmjlthaqq.html

[R47] sed 单行替换
来源：http://hz.xylfe.cn/gtjcrrhajm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jlsjyb.cn/gtjybzkhop.html

[R48] awk 取指定列
来源：http://hz.guannengcc.top/gtysvibhes.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinyuanbaomall.cn/gtszztudyo.html

[R49] awk 带条件
来源：http://hz.0kj1m.cn/gtppzlpsjf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangdashe.top/gtoybftehc.html

[R50] awk 求和
来源：http://hz.ywan-chungtsiang.top/gtjoijcuur.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gtbpkhbpyp.html

[R51] 排序去重取前几
来源：http://hz.pycfn.com/gtaghahfnk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nanxuanxn.top/gtpdobbntg.html

[R52] 统计行数
来源：http://hz.zhoulong.xyz/gtyzbcdksh.html

wc -l a.txt
来源：http://hz.fengsongda.top/gtmxusccjy.html

[R53] 查看文件头与实时尾
来源：http://hz.wangshuangyany.cn/gtulbyqynd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnxiangtu.top/gtiefnvxql.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gthefmpmxe.html

diff a.txt b.txt
来源：http://hz.meibo888.top/gtzhrgenyd.html

[R55] 压缩与解压
来源：http://hz.sxryk.cn/gtflliocai.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnxiangtu.top/gtrqvwbymp.html

[R56] 远程拷贝
来源：http://hz.c1oappe.top/gtdqbzmpwt.html

scp file user@host:/path/
来源：http://hz.hammf.cn/gtwfobcvfk.html

[R57] 远程执行命令
来源：http://hz.pycfn.com/gtmqlgaqwc.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangkeji.top/gtpkwluwcu.html

[R58] 下载文件
来源：http://hz.quarkkingdee.top/gtnkebqnnj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pycfn.com/gtmxjjkhyl.html

[R59] 发 POST JSON
来源：http://hz.quarkkingdee.top/gtuyvgugcd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hongshengwenyu.top/gtqgbqvhox.html

[R60] 只看 HTTP 状态码
来源：http://hz.yuxming.cn/gtrypyrkrg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shuidangran.top/gtnjpmxwlc.html

[R61] 磁盘占用
来源：http://hz.hammf.cn/gtdvmjuwrt.html

df -h;  du -sh *
来源：http://hz.pycfn.com/gtmqtzfngj.html

[R62] 找最占空间的文件
来源：http://hz.sysykeji.top/gtbluuqsuw.html

du -ah . | sort -rh | head -10
来源：http://hz.xuetiantiany.cn/gtekbtqfrq.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtdcrfwwky.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtmnzkxbgv.html

[R64] 结束进程
来源：http://hz.cheryme.top/gtkjcalusg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gtmudcwqsf.html

[R65] 查看端口占用
来源：http://hz.daxiang520.top/gttpuikqmr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinghuilouyu.cn/gtstonnkxb.html

[R66] 定时任务
来源：http://hz.birdmap.top/gtkkjzsejm.html

crontab -e;  crontab -l
来源：http://hz.0kj1m.cn/gtmauronrd.html

[R67] 生成随机十六进制串
来源：http://hz.nanxinkj.top/gtyrhbebjd.html

openssl rand -hex 16
来源：http://hz.ppjwa.cn/gtjevgkwoh.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtkevelkur.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jinqigufen.top/gtxtmlhpgv.html

[R69] 生成随机密码
来源：http://hz.quarkkingdee.top/gtgzlcozqe.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinghuilouyu.cn/gtuffanojd.html

[R70] 时间戳与互转
来源：http://hz.svipenyu.cn/gtezeudsqg.html

date +%s;  date -d @1700000000
来源：http://hz.jqgfzy.top/gtqdhheago.html

[R71] 日期格式化
来源：http://hz.ivvv.top/gthnmvksaj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jiagoushi.top/gtgkcphgyk.html

[R72] 等待端口就绪
来源：http://hz.hnxiangtu.top/gtxtmlrvlz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtjqgjvilh.html

[R73] 分割大日志
来源：http://hz.aizwys.cn/gtxrexwylm.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gttmyldtrq.html

[R74] 批量重命名
来源：http://hz.yuanzhike.top/gtgwqcskmp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.snrcjt.cn/gtwccszvml.html

[R75] 导出环境变量
来源：http://hz.fzhhl.top/gtdhbumldx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nwbrower.top/gtxeprvdsr.html

[R76] 使用临时文件
来源：http://hz.havefunace.top/gtsvjconbw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.aibaodan.cn/gthbrurcgc.html

[R77] 读取用户输入
来源：http://hz.cqqwz.cn/gtqwdbjbyq.html

read -rp "请输入: " ans
来源：http://hz.zhaomingkeji.xyz/gtpdqyqgpg.html

[R78] 交互式菜单
来源：http://hz.zhongyouzk.top/gtyxselbie.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zdqjudy.top/gtcluwbnhf.html

[R79] 解析命令行选项
来源：http://hz.haohaochexian.top/gtnelsbcqt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenlongwang.top/gtlrexalwr.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gtxfbzjpdb.html

time ./run.sh
来源：http://hz.wangdashe.top/gtybibujyl.html

================================================================================
来源：http://hz.cheryme.top/gtfktylcag.html

S. C / C++ 专题
来源：http://hz.nanxuanxn.top/gthtzbsrey.html

================================================================================
来源：http://hz.yuanzhike.top/gtakszskzg.html

[S01] C：Hello World
来源：http://hz.gogol.net.cn/gtrqsgjbzf.html

#include <stdio.h>
来源：http://hz.zhengqikj.top/gtumpuingr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dashuyun.cn/gthbeywobi.html

[S02] C：变量与格式化输出
来源：http://hz.zhongyouzk.top/gtcoufeaur.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gtdnnhtqyp.html

[S03] C：读入整数
来源：http://hz.hongshengwenyu.top/gttzfgmmgv.html

int x; scanf("%d", &x);
来源：http://hz.svipenyu.cn/gtmjmozekm.html

[S04] C：字符串复制
来源：http://hz.daxiang520.top/gtahppuexz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gzhubu.top/gtfpnkrhln.html

[S05] C：字符串长度
来源：http://hz.gotoacloud.top/gtgmfucmwl.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtthsvgvzr.html

[S06] C：字符串比较
来源：http://hz.pengpengdd.cyou/gtmcorjbvd.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gtvbetnjvd.html

[S07] C：数组遍历求和
来源：http://hz.shangyingyoupin.top/gtesfwnlqd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.316326.xyz/gteqigteio.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtsuzxexjt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hysaishi.cn/gtqgndguen.html

[S09] C：结构体定义与初始化
来源：http://hz.ehwqpu.com/gtitrtlxpa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigufen.top/gtlzytahrx.html

[S10] C：指针与解引用
来源：http://hz.guannengcc.top/gtdfencyjx.html

int *p = &a;  *p = 5;
来源：http://hz.vqdsnc.cn/gtjvpjkktk.html

[S11] C：逐行读文件
来源：http://hz.tanke756.top/gtrujuzhnd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.svipenyu.cn/gtvvhldcxf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.c1oappe.top/gthutqkluh.html

fclose(f);
来源：http://hz.316326.xyz/gtjivovqhv.html

[S12] C：写文件
来源：http://hz.shanyushiyangtech.top/gtxsuedngl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tianlin.xyz/gtjfjodouy.html

[S13] C：宏定义
来源：http://hz.xinyue.icu/gtectdazcd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hywenlv.cn/gtwxwawnmw.html

[S14] C：枚举
来源：http://hz.316326.xyz/gtuxpzhmya.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gtlpusvrym.html

[S15] C：类型转换
来源：http://hz.iojbl.cn/gtlvberwyn.html

(double) a / b
来源：http://hz.c1oappe.top/gtceubkjif.html

[S16] C：位操作置位
来源：http://hz.snrcjt.cn/gtmqlhnble.html

x |= (1 << 3);
来源：http://hz.zhiwuduotai.top/gtdswusmyn.html

[S17] C：安全拼接字符串
来源：http://hz.jinghuilouyu.cn/gtqkkqqqii.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.vqdsnc.cn/gtlvslvnky.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gtbatgcnsf.html


<!-- 参考信息 -->