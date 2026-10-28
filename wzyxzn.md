代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.zhoulong.xyz/gtaolohjjb.html

[Q50] 批量更新
来源：http://hz.jinqigufen.top/gtztfhabdj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gaohongyu789.top/gtttaqkqvg.html

[Q51] 用子查询更新
来源：http://hz.daria6918.cn/gtvvyjlzyr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.sweek.top/gtekrtgdrw.html

[Q52] 删除指定行
来源：http://hz.gotoacloud.top/gtqwlozuvb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.smart0.xyz/gtyiihihzd.html

[Q53] 按条件删除
来源：http://hz.hnxiangtu.top/gtbqqdilge.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.cdnleiting.top/gtcruakuia.html

[Q54] 清空表
来源：http://hz.ydzc1.top/gtsopbueoh.html

TRUNCATE TABLE logs;
来源：http://hz.aizwys.cn/gttkhgaggc.html

[Q55] 排名（并列占位）
来源：http://hz.shangyingyoupin.top/gtlvazqzak.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.wangdashe.top/gtrhilazod.html

[Q56] 密集排名（并列不占位）
来源：http://hz.kuanghao11.cn/gtqsxyumim.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.zhijiandao.cn/gtvyqayxzm.html

[Q57] 行号
来源：http://hz.hywenlv.cn/gtalmpqgcl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cashguo.top/gtloqmmaxp.html

[Q58] 累计求和
来源：http://hz.316326.xyz/gtmbxwofmn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xylfe.cn/gtmuugwcwo.html

[Q59] 分组内累计
来源：http://hz.ivvv.top/gttmsvwaia.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zhaomingkeji.xyz/gthqsoinbd.html

[Q60] 取上一行 / 下一行
来源：http://hz.gaohongyu789.top/gtzusklqft.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.chenjidiqi.icu/gtjomuozib.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.52xcode.cn/gtzwizzjlw.html

[Q61] 移动平均
来源：http://hz.quarkkingdee.top/gttlbdjvub.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hammf.cn/gtmvvbfols.html

[Q62] 分组占比
来源：http://hz.shanyushiyangtech.top/gtkmvdglbv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yvedp.cn/gtdpskueln.html

[Q63] 开启事务
来源：http://hz.hnxiangtu.top/gtsphemire.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhongyouzk.top/gtzmylfhoq.html

[Q64] 提交事务
来源：http://hz.zycfv.cn/gtkwwgwphu.html

COMMIT;
来源：http://hz.zhengqikj.top/gtffxklpeg.html

[Q65] 回滚事务
来源：http://hz.hammf.cn/gtxplgexnu.html

ROLLBACK;
来源：http://hz.jinyuanbaomall.cn/gtoeapbvqg.html

[Q66] 行锁查询
来源：http://hz.hfpthk.cn/gtocflmvje.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gogol.net.cn/gtgwubwoss.html

[Q67] 设置隔离级别
来源：http://hz.cashguo.top/gtzetnohat.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yj20258888.top/gtgvcctpri.html

[Q68] 保存点
来源：http://hz.haohaochexian.top/gtwcomhmqg.html

SAVEPOINT sp1;
来源：http://hz.daria6918.cn/gtqswbelnr.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gtkndjzluy.html

[Q69] 查看执行计划
来源：http://hz.nanxinkj.top/gtduzzkapn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jqgufenzy.top/gtzajmueev.html

[Q70] 更新统计信息
来源：http://hz.ehwqpu.com/gtcqctdnhn.html

ANALYZE TABLE users;
来源：http://hz.daria6918.cn/gtsuucahms.html

[Q71] 查看建表语句
来源：http://hz.smart0.xyz/gtobrbrxbb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.pycfn.com/gtgcchnlci.html

[Q72] 查看索引
来源：http://hz.xziqi.cn/gtsrcjasmb.html

SHOW INDEX FROM users;
来源：http://hz.yonumen.top/gtczlicoie.html

[Q73] 查看表状态
来源：http://hz.sxryk.cn/gtegihocug.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.yuanzhike.top/gtlfjqgrsz.html

[Q74] 强制使用索引
来源：http://hz.c1oappe.top/gtavxgsuuu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xinyue.icu/gtpysuusrb.html

[Q75] 日期格式化
来源：http://hz.jqgufenzy.top/gtbrecewyk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guowangkeji.top/gtqzyatmoe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sweek.top/gtmeknkpdq.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gthamuvsgn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.gaohongyu789.top/gtutuaklpe.html

[Q77] 时间加减
来源：http://hz.xziqi.cn/gtcxnbjscs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.svipenyu.cn/gtkchwmcil.html

[Q78] 当前时间
来源：http://hz.chenzaomai.com/gtyqnlvxcv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yanxiufei.cn/gtlhyuqkym.html

[Q79] 字符串拼接
来源：http://hz.yj20258.top/gttvssnxxz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.9152youxi.cn/gtspjebcaf.html

[Q80] 字符串截取
来源：http://hz.c1oappe.top/gtbtomuuks.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hnqzz.top/gtgbkdzyvz.html

[Q81] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gttpxtabhl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.daxiang520.top/gtqvmquwdi.html

[Q82] 字符长度与字节长度
来源：http://hz.yuanzhike.top/gttuzqpjag.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtzoiesltp.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangtech.top/gtycgqgbdm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.dianchejie.cn/gttougsjzr.html

[Q84] 去除首尾空格
来源：http://hz.ehwqpu.com/gtfgahjkux.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gtvwxmvnck.html

[Q85] 数值取整
来源：http://hz.xziqi.cn/gtgudgydmh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.shzxlz.cn/gtojpnwzei.html

[Q86] 读取 JSON 字段
来源：http://hz.hnqzz.top/gtrlimgrjo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhongyouzk.top/gtsmjhfwfr.html

[Q87] JSON 字段做条件
来源：http://hz.yongpay.top/gtkcidjzsa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.mhx1999.top/gtyukjpwnr.html

[Q88] 行转列（条件聚合）
来源：http://hz.pycfn.com/gtvnyqiqge.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jqgfzy.top/gtmliexsye.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gogol.net.cn/gtkfhiqddu.html

[Q89] 判断表是否存在
来源：http://hz.ydjk.org.cn/gtczjekvjd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tianlin.xyz/gtqosieakn.html

[Q90] 生成序号列
来源：http://hz.jqgfzy.top/gtyraeuqcl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.dashuyun.cn/gtspktjmww.html

================================================================================
来源：http://hz.guannengcc.top/gtygmljfls.html

R. Bash 专题
来源：http://hz.fengsongda.top/gtoyodcfmw.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgdgnrzyn.html

[R01] shebang 与严格模式
来源：http://hz.yj20258888.top/gtontoeeoa.html

#!/usr/bin/env bash
来源：http://hz.xingfuxueyuan.xyz/gtrieumqfa.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtwyqxldgl.html

[R02] 变量赋值与使用
来源：http://hz.sxryk.cn/gthjfnpfwd.html

name="Tom"; echo "$name"
来源：http://hz.jlsjyb.cn/gtkqglytgf.html

[R03] 只读变量
来源：http://hz.zhijiandao.cn/gtmfzzxbxq.html

readonly PI=3.14
来源：http://hz.xuetiantiany.cn/gtwfuhhbab.html

[R04] 位置参数
来源：http://hz.wangdashe.top/gtipshwoui.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shuidangran.top/gtkjttfeft.html

[R05] 参数默认值
来源：http://hz.gotoacloud.top/gtutgvrhne.html

name="${1:-default}"
来源：http://hz.bjfxy.top/gtxtjfjvrm.html

[R06] 判断命令是否存在
来源：http://hz.zycfv.cn/gttnkdeakv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ybcxt.top/gtgsltvrgu.html

[R07] if 判断文件
来源：http://hz.jlsjyb.cn/gtynaqklcg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangdashe.top/gtlnoghmxp.html

[R08] 数值比较
来源：http://hz.ydzc1.top/gtufnwdztx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yueranfly.top/gtbunjmnid.html

[R09] 字符串比较
来源：http://hz.xylfe.cn/gtbfngbluf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aizwys.cn/gtnkwdftry.html

[R10] 正则匹配
来源：http://hz.wangdashe.top/gtmrocaxwv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jlsjyb.cn/gtosoyabnm.html

[R11] case 多分支
来源：http://hz.wangshuangyany.cn/gtpetkgruw.html

case "$1" in
来源：http://hz.zycfv.cn/gtmqqyvsow.html

start) echo "启动" ;;
来源：http://hz.c1oappe.top/gtkvtbqwde.html

stop)  echo "停止" ;;
来源：http://hz.svipenyu.cn/gtbducmsuw.html

*)     echo "未知命令" ;;
来源：http://hz.chenlongwang.top/gtobtkeikp.html

esac
来源：http://hz.chenzaomai.com/gtqyxsdgnk.html

[R12] for 遍历文件
来源：http://hz.yuanzhike.top/gtcxomgxuc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.andypj.xyz/gtekcrwskh.html

[R13] for 计数循环
来源：http://hz.aizwys.cn/gttisjuzvn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtkkmtqauw.html

[R14] C 风格 for
来源：http://hz.ivvv.top/gtegfyibdu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.iojbl.cn/gtfuqmbbnz.html

[R15] while 逐行读文件
来源：http://hz.gzhubu.top/gtzomihxbf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gzhubu.top/gtbcxrmmtd.html

[R16] until 等待条件
来源：http://hz.pengpengdd.cyou/gtavixihvi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.aibaodan.cn/gtoheckipg.html

[R17] 数组定义与取值
来源：http://hz.gogol.net.cn/gtdulsumea.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgufenzy.top/gtbowhsblr.html

[R18] 遍历数组
来源：http://hz.nanxuanxn.top/gtcuyflmtx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.sweek.top/gtdrnoggsv.html

[R19] 数组长度
来源：http://hz.tanke756.top/gtipqnljxh.html

echo "${#arr[@]}"
来源：http://hz.hongshengwenyu.top/gtzhjulstm.html

[R20] 关联数组（字典）
来源：http://hz.jinqigfzy.top/gtjpxqvixu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hongshengwenyu.top/gtjjtsvium.html

[R21] 字符串长度
来源：http://hz.chenzaomai.com/gtkmsjgrwj.html

echo "${#s}"
来源：http://hz.c1oappe.top/gtwbmfinjl.html

[R22] 截取子串
来源：http://hz.bjfxy.top/gtmvysxfru.html

echo "${s:0:5}"
来源：http://hz.xuetiantiany.cn/gtvllsxvcn.html

[R23] 字符串替换
来源：http://hz.daxiang520.top/gthlastmjl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hywenlv.cn/gtnqdkchyt.html

[R24] 大小写转换
来源：http://hz.sufxvd.cn/gtwmjklcus.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shzxlz.cn/gtawqkqolx.html

[R25] 去后缀 / 去前缀
来源：http://hz.redwolf501.top/gthwmvhaiy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xuanzx.com/gtzfqfroqp.html

[R26] 命令替换
来源：http://hz.daxiang520.top/gtmqvtqecv.html

now=$(date +%F); echo "$now"
来源：http://hz.birdmap.top/gttruoryza.html

[R27] 算术展开
来源：http://hz.daria6918.cn/gtvmimxnjf.html

echo $((1 + 2 * 3))
来源：http://hz.zhoulong.xyz/gtojxywjmt.html

[R28] 浮点运算
来源：http://hz.hywenlv.cn/gtmxqdckgz.html

echo "scale=2; 10/3" | bc
来源：http://hz.daxiang520.top/gtmnwaokkh.html

[R29] 定义函数
来源：http://hz.gogol.net.cn/gtvrwpspva.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenjidiqi.icu/gtnicqevln.html

[R30] 函数返回状态码
来源：http://hz.gaohongyu789.top/gtgwpetajv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jinyuanbaomall.cn/gtgnzpjxie.html

[R31] 局部变量
来源：http://hz.gaohongyu789.top/gtilyjcbie.html

f() { local x=1; echo "$x"; }
来源：http://hz.kuanghao11.cn/gtqdylfckr.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gtlqytvvmy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.bjfxy.top/gtpevixqtw.html

[R33] 捕获错误并提示行号
来源：http://hz.chenlongwang.top/gtwlkpwygr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.52xcode.cn/gtbnknswre.html

[R34] 退出时清理
来源：http://hz.sysykeji.top/gtnzdczmex.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258.top/gtxprrtvsb.html

[R35] 后台执行并等待
来源：http://hz.cashguo.top/gtrmhvapgd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cucudq.cn/gtwnnegbjc.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtjguhfajs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.havefunace.top/gtpnzkmifv.html

[R37] 把输出赋给变量
来源：http://hz.cashguo.top/gtbhqwmqgr.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtwyqnwwig.html

[R38] 管道串联
来源：http://hz.xziqi.cn/gtyajzegso.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuanzx.com/gtcafrknrw.html

[R39] 重定向标准输出与错误
来源：http://hz.quarkkingdee.top/gtyvndebrl.html

cmd > out.log 2>&1
来源：http://hz.yanxiufei.cn/gtcqokpgit.html

[R40] 追加写日志
来源：http://hz.cdnleiting.top/gtiidbsnhc.html

echo "log" >> out.log
来源：http://hz.xingfuxueyuan.xyz/gtnkluxueo.html

[R41] 丢弃输出
来源：http://hz.gotoacloud.top/gtkgyvlryx.html

cmd >/dev/null 2>&1
来源：http://hz.cucudq.cn/gtsqpetugo.html

[R42] 输入重定向
来源：http://hz.zycfv.cn/gtcjvwsiux.html

wc -l < a.txt
来源：http://hz.jinqigufen.top/gtvsuvgfqv.html

[R43] 按名字查找文件
来源：http://hz.yvedp.cn/gtzuxyvshv.html

find . -name "*.log" -type f
来源：http://hz.guowangkeji.top/gtribatpyh.html

[R44] 按修改时间查找
来源：http://hz.quarkkingdee.top/gtzotdxvbn.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtkuvpergg.html

[R45] 批量删除
来源：http://hz.pengpengdd.cyou/gtbzufspnu.html

find . -name "*.tmp" -delete
来源：http://hz.xuanzx.com/gtutyutsxt.html

[R46] 递归替换文件内容
来源：http://hz.fzhhl.top/gtakicclzh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gtkwdnqoqu.html

[R47] sed 单行替换
来源：http://hz.9152youxi.cn/gtevadvzms.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.vqdsnc.cn/gtagduuxzf.html

[R48] awk 取指定列
来源：http://hz.zhaomingkeji.xyz/gtfqglfyaq.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigufen.top/gtddmvtoje.html

[R49] awk 带条件
来源：http://hz.tianlin.xyz/gtvgxkjvgf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.quarkkingdee.top/gtznhqkdsz.html

[R50] awk 求和
来源：http://hz.yonumen.top/gtgocjujxr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nwbrower.top/gtnmvcjtjj.html

[R51] 排序去重取前几
来源：http://hz.kuanghao11.cn/gtvakykncq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinqigufen.top/gtfgiwctfp.html

[R52] 统计行数
来源：http://hz.guannengcc.top/gtossyreyb.html

wc -l a.txt
来源：http://hz.shanyushiyangtech.top/gtjreghusx.html

[R53] 查看文件头与实时尾
来源：http://hz.0kj1m.cn/gtdnalqodq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.pengpengdd.cyou/gtcvdvaasb.html

[R54] 比较两个文件
来源：http://hz.ydzc1.top/gtydxkyrmh.html

diff a.txt b.txt
来源：http://hz.xuanzx.com/gtqtdfsdqv.html

[R55] 压缩与解压
来源：http://hz.haohaochexian.top/gtgkxiwryd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gzhubu.top/gtwrhofdsb.html

[R56] 远程拷贝
来源：http://hz.bjfxy.top/gtvapoyeoh.html

scp file user@host:/path/
来源：http://hz.sysykeji.top/gtkumgfept.html

[R57] 远程执行命令
来源：http://hz.cdnleiting.top/gtudvzlkib.html

ssh user@host 'uptime'
来源：http://hz.zycfv.cn/gticcxmkds.html

[R58] 下载文件
来源：http://hz.yj202588.top/gtizrpkcgi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.dashuyun.cn/gtnuwxltta.html

[R59] 发 POST JSON
来源：http://hz.sufxvd.cn/gtfzvqwjue.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuanzhike.top/gtlslxiezr.html

[R60] 只看 HTTP 状态码
来源：http://hz.sxryk.cn/gtrvulmtgh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenlongwang.top/gtrzfevwpv.html

[R61] 磁盘占用
来源：http://hz.xuetiantiany.cn/gteqbiiide.html

df -h;  du -sh *
来源：http://hz.shzxlz.cn/gtqhtrvjbh.html

[R62] 找最占空间的文件
来源：http://hz.mhx1999.top/gtmhxpsfce.html

du -ah . | sort -rh | head -10
来源：http://hz.yangfankeji.com/gtuwwsxisl.html

[R63] 内存与进程
来源：http://hz.cdnleiting.top/gtczfdybnx.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258888.top/gthiyzcltf.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtsreoftvt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuxming.cn/gtgkpbrcis.html

[R65] 查看端口占用
来源：http://hz.nanxinkj.top/gttdcggchb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydjk.org.cn/gtzhszcamu.html

[R66] 定时任务
来源：http://hz.cashguo.top/gtswuywmnl.html

crontab -e;  crontab -l
来源：http://hz.yj20258888.top/gtpqtwbmmd.html

[R67] 生成随机十六进制串
来源：http://hz.dashuyun.cn/gtsqqgpswh.html

openssl rand -hex 16
来源：http://hz.hongshengwenyu.top/gtmbtpdhtc.html

[R68] 计算文件校验值
来源：http://hz.gzhubu.top/gtqlkgkhpg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cdnleiting.top/gtjvokvkvp.html

[R69] 生成随机密码
来源：http://hz.bjfxy.top/gtfxcgoosq.html

head -c 16 /dev/urandom | base64
来源：http://hz.iojbl.cn/gtbmkerqvj.html

[R70] 时间戳与互转
来源：http://hz.sweek.top/gtzbasbblc.html

date +%s;  date -d @1700000000
来源：http://hz.quarkkingdee.top/gtpijreqal.html

[R71] 日期格式化
来源：http://hz.guowangkeji.top/gtnevvnvgo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sxryk.cn/gtsqlxtehe.html

[R72] 等待端口就绪
来源：http://hz.shangyingyoupin.top/gtdiniznqf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.bjfxy.top/gtzugjuyzx.html

[R73] 分割大日志
来源：http://hz.zhijiandao.cn/gtplrjeypq.html

split -l 1000 big.log part_
来源：http://hz.9152youxi.cn/gtrfybqtei.html

[R74] 批量重命名
来源：http://hz.jqgfzy.top/gtguhsxlpl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jqgufenzy.top/gtsqltcybg.html

[R75] 导出环境变量
来源：http://hz.aibaodan.cn/gtkkvkwvvu.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.kuanghao11.cn/gtgtuhzvul.html

[R76] 使用临时文件
来源：http://hz.hongshengwenyu.top/gtghcyqtqd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtcbdytjam.html

[R77] 读取用户输入
来源：http://hz.yanxiufei.cn/gtlbzvmzvy.html

read -rp "请输入: " ans
来源：http://hz.zycfv.cn/gthkkfakdh.html

[R78] 交互式菜单
来源：http://hz.zhongyouzk.top/gtcgigsscj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtpygfhyty.html

[R79] 解析命令行选项
来源：http://hz.vqdsnc.cn/gtxdliqthc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shangyingyoupin.top/gtcnmfabgq.html

[R80] 查看脚本执行耗时
来源：http://hz.jyoumei.cn/gtsbwotrho.html

time ./run.sh
来源：http://hz.xuetiantiany.cn/gtmednzhlf.html

================================================================================
来源：http://hz.gaohongyu789.top/gtypdidojb.html

S. C / C++ 专题
来源：http://hz.sweek.top/gtizvzyhht.html

================================================================================
来源：http://hz.daxiang520.top/gtauvkucvb.html

[S01] C：Hello World
来源：http://hz.52xcode.cn/gtghrzozha.html

#include <stdio.h>
来源：http://hz.yonumen.top/gtueekyket.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ehwqpu.com/gtbnmfulyx.html

[S02] C：变量与格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtpoflrjfo.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgfzy.top/gtiiehtwwn.html

[S03] C：读入整数
来源：http://hz.ehwqpu.com/gtfeutxrhm.html

int x; scanf("%d", &x);
来源：http://hz.ehwqpu.com/gtqtckvzin.html

[S04] C：字符串复制
来源：http://hz.yanxiufei.cn/gtnogmlize.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cdnleiting.top/gteqtufqcv.html

[S05] C：字符串长度
来源：http://hz.jqgufenzy.top/gtzmvnugfh.html

strlen(s)
来源：http://hz.sysykeji.top/gtawwdtqjd.html

[S06] C：字符串比较
来源：http://hz.guannengcc.top/gtxfkjenzi.html

strcmp(a, b) == 0
来源：http://hz.9152youxi.cn/gtvdjqpukp.html

[S07] C：数组遍历求和
来源：http://hz.aizwys.cn/gtzvuaxbkp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hammf.cn/gtexgiqknn.html

[S08] C：动态内存分配与释放
来源：http://hz.cdnleiting.top/gtpydtekgs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.wangdashe.top/gtqzcfqdhd.html

[S09] C：结构体定义与初始化
来源：http://hz.yangfankeji.com/gtjktpttyg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.chenzaomai.com/gtnzpymasa.html

[S10] C：指针与解引用
来源：http://hz.hnqzz.top/gtptjaorzk.html

int *p = &a;  *p = 5;
来源：http://hz.snrcjt.cn/gtchsvhsjg.html

[S11] C：逐行读文件
来源：http://hz.sufxvd.cn/gtubawxjqv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.bjfxy.top/gtojeyrlvw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gaohongyu789.top/gtqhyqhpxq.html

fclose(f);
来源：http://hz.yangfankeji.com/gtczeddabg.html

[S12] C：写文件
来源：http://hz.yuxming.cn/gtyqwuuekc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ppjwa.cn/gtaovzgfpj.html

[S13] C：宏定义
来源：http://hz.shanyushiyangkeji.top/gtvdajmgzk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgufenzy.top/gtubpqtivc.html

[S14] C：枚举
来源：http://hz.shanyushiyangtech.top/gtbvpampgk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenzaomai.com/gtxkdziqtl.html

[S15] C：类型转换
来源：http://hz.wangshuangyany.cn/gtojfwrpje.html

(double) a / b
来源：http://hz.xylfe.cn/gtqkomdksb.html

[S16] C：位操作置位
来源：http://hz.0kj1m.cn/gtitaqdxem.html

x |= (1 << 3);
来源：http://hz.xuetiantiany.cn/gtdtunozls.html

[S17] C：安全拼接字符串
来源：http://hz.zhiwuduotai.top/gtzetjfigg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xylfe.cn/gtfvstzvhd.html

[S18] C：命令行参数
来源：http://hz.hfpthk.cn/gtpizweczn.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtuisccoqj.html

[S19] C：快速排序
来源：http://hz.smart0.xyz/gtbmusthfq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtethvyhnz.html

[S20] C：二分查找
来源：http://hz.yvedp.cn/gtxqvynprj.html


<!-- 参考信息 -->