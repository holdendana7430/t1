代发 wailian999

[Q61] 移动平均
来源：http://hz.jianghu66.top/gtxxvqksqc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhiwuduotai.top/gtnikfwqkb.html

[Q62] 分组占比
来源：http://hz.guannengcc.top/gtcnlccovx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yonumen.top/gtfklajepr.html

[Q63] 开启事务
来源：http://hz.zycfv.cn/gtwwsuiewp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tian-w.cn/gtigzhqwzx.html

[Q64] 提交事务
来源：http://hz.jlsjyb.cn/gtzlcitnsp.html

COMMIT;
来源：http://hz.xuanzx.com/gtblawhflw.html

[Q65] 回滚事务
来源：http://hz.guowangkeji.top/gtsuxwugtx.html

ROLLBACK;
来源：http://hz.sysykeji.top/gtjstazqeg.html

[Q66] 行锁查询
来源：http://hz.jianghu66.top/gtutqitlrm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.smart0.xyz/gtklrnzzff.html

[Q67] 设置隔离级别
来源：http://hz.zycfv.cn/gthpvjioaw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yvedp.cn/gtzijcukvw.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtfuttxbkq.html

SAVEPOINT sp1;
来源：http://hz.cdnleiting.top/gtejibkxvk.html

ROLLBACK TO sp1;
来源：http://hz.52xcode.cn/gtacooyevn.html

[Q69] 查看执行计划
来源：http://hz.aibaodan.cn/gtxeczwhrf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yj20258888.top/gtfnjysnsa.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtvqglgfbf.html

ANALYZE TABLE users;
来源：http://hz.hysaishi.cn/gtnmiocgut.html

[Q71] 查看建表语句
来源：http://hz.xziqi.cn/gtassgkxzf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.yueranfly.top/gtoayjtewh.html

[Q72] 查看索引
来源：http://hz.ivvv.top/gtcmmofacb.html

SHOW INDEX FROM users;
来源：http://hz.ehwqpu.com/gtooavhqaq.html

[Q73] 查看表状态
来源：http://hz.xuanzx.com/gttqvskadm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cdnleiting.top/gtllroysko.html

[Q74] 强制使用索引
来源：http://hz.52xcode.cn/gtpssowhtj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinqigfzy.top/gtegmpntpb.html

[Q75] 日期格式化
来源：http://hz.guowangkeji.top/gthjigrlda.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuetiantiany.cn/gtibjiyxsx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258888.top/gtehurqhkz.html

[Q76] 按天统计
来源：http://hz.daria6918.cn/gtjehnfwfh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.dashuyun.cn/gtfoymnrsh.html

[Q77] 时间加减
来源：http://hz.sweek.top/gtihkozbhh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnqzz.top/gthtwhgyao.html

[Q78] 当前时间
来源：http://hz.tian-w.cn/gtfsskjzho.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.chenjidiqi.icu/gtclyohnxy.html

[Q79] 字符串拼接
来源：http://hz.ybcxt.top/gtygwfsmeh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.wangdashe.top/gtplgjkafl.html

[Q80] 字符串截取
来源：http://hz.cashguo.top/gtflhxraxn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jianghu66.top/gtzevqshgz.html

[Q81] 字符串替换
来源：http://hz.haohaochexian.top/gtayisgytc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ybcxt.top/gtrlvvulic.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtfkpnhfqw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.cheryme.top/gtnookclhu.html

[Q83] 大小写转换
来源：http://hz.yanxiufei.cn/gttqbobfoz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gaohongyu789.top/gtfwndkxwo.html

[Q84] 去除首尾空格
来源：http://hz.jinghuilouyu.cn/gtedsbudwh.html

SELECT TRIM(name) FROM users;
来源：http://hz.9152youxi.cn/gtwttlreex.html

[Q85] 数值取整
来源：http://hz.jianghu66.top/gtqjwyakal.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nanxinkj.top/gtxfvdiamg.html

[Q86] 读取 JSON 字段
来源：http://hz.zdqjudy.top/gtdqvyqjue.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.shzxlz.cn/gtvczphdhq.html

[Q87] JSON 字段做条件
来源：http://hz.snrcjt.cn/gtqblopani.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nwbrower.top/gteqvbkynv.html

[Q88] 行转列（条件聚合）
来源：http://hz.daria6918.cn/gthldtqyst.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gtsziwpkeb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenjidiqi.icu/gtnvtzvfou.html

[Q89] 判断表是否存在
来源：http://hz.guannengcc.top/gtakbdsuig.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dianchejie.cn/gtzhiyjvja.html

[Q90] 生成序号列
来源：http://hz.yongpay.top/gtpzecjkli.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yongpay.top/gtubjtqvkb.html

================================================================================
来源：http://hz.haohaochexian.top/gtysrvvkdk.html

R. Bash 专题
来源：http://hz.tian-w.cn/gtkzrtxpxu.html

================================================================================
来源：http://hz.hnxiangtu.top/gthllqtzcj.html

[R01] shebang 与严格模式
来源：http://hz.tian-w.cn/gtoutdqzre.html

#!/usr/bin/env bash
来源：http://hz.zhijiandao.cn/gtwdzuvizs.html

set -euo pipefail
来源：http://hz.wangdashe.top/gtjjtrnjlb.html

[R02] 变量赋值与使用
来源：http://hz.ybcxt.top/gtgmvpcudk.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangtech.top/gtdaekdjdf.html

[R03] 只读变量
来源：http://hz.birdmap.top/gtuhrqqndm.html

readonly PI=3.14
来源：http://hz.xuetiantiany.cn/gtwroqsiko.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gtadswcfan.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.smart0.xyz/gtasgriqjz.html

[R05] 参数默认值
来源：http://hz.hnqzz.top/gtlyvtcpvn.html

name="${1:-default}"
来源：http://hz.yonumen.top/gtndidndqs.html

[R06] 判断命令是否存在
来源：http://hz.yj20258.top/gtnthsgnyp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.daria6918.cn/gtxeuoeixv.html

[R07] if 判断文件
来源：http://hz.kuanghao11.cn/gthikvesec.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.chenlongwang.top/gtbumkchwv.html

[R08] 数值比较
来源：http://hz.nanxuanxn.top/gtlybaejxe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.fengsongda.top/gtvknvjtvq.html

[R09] 字符串比较
来源：http://hz.zdqjudy.top/gtyufglsxw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.nanxinkj.top/gttkoipuge.html

[R10] 正则匹配
来源：http://hz.daxiang520.top/gtajwfynak.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jyoumei.cn/gtambadhds.html

[R11] case 多分支
来源：http://hz.ehwqpu.com/gtvafaumyj.html

case "$1" in
来源：http://hz.snrcjt.cn/gtefwadfsv.html

start) echo "启动" ;;
来源：http://hz.hammf.cn/gtutilqijf.html

stop)  echo "停止" ;;
来源：http://hz.chenlongwang.top/gtmyiwdylg.html

*)     echo "未知命令" ;;
来源：http://hz.yj202588.top/gtdnyswoel.html

esac
来源：http://hz.nanxuanxn.top/gtttrbvssh.html

[R12] for 遍历文件
来源：http://hz.zhengqikj.top/gtwklbmkqf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hnqzz.top/gtjqbvrmdm.html

[R13] for 计数循环
来源：http://hz.yj20258888.top/gtvsaxlbpc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gzhubu.top/gtmhldlnkj.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gtawspqefj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.bjfxy.top/gtzqzroguk.html

[R15] while 逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtkcitqwoa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jlsjyb.cn/gtuhrzkwfe.html

[R16] until 等待条件
来源：http://hz.mhx1999.top/gtejsktwbj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sxryk.cn/gtwzedruwn.html

[R17] 数组定义与取值
来源：http://hz.yongpay.top/gtagusxloa.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daria6918.cn/gtwyngazpn.html

[R18] 遍历数组
来源：http://hz.smart0.xyz/gtsimqadmy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yueranfly.top/gtdlygzrop.html

[R19] 数组长度
来源：http://hz.shzxlz.cn/gtedooqozx.html

echo "${#arr[@]}"
来源：http://hz.vqdsnc.cn/gteeibneya.html

[R20] 关联数组（字典）
来源：http://hz.jianghu66.top/gtefztknez.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.sxryk.cn/gtynybupvj.html

[R21] 字符串长度
来源：http://hz.xziqi.cn/gtirkpimzt.html

echo "${#s}"
来源：http://hz.sweek.top/gtlkkcqdzu.html

[R22] 截取子串
来源：http://hz.wangshuangyany.cn/gtvliolrui.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtngppjesf.html

[R23] 字符串替换
来源：http://hz.zhiwuduotai.top/gtmqgjdgzp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hongshengwenyu.top/gtbyabnlxx.html

[R24] 大小写转换
来源：http://hz.zhoulong.xyz/gtvcbpgach.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sysykeji.top/gtjbktcndw.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258888.top/gtbocxecvs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fengsongda.top/gtwbknazwa.html

[R26] 命令替换
来源：http://hz.cheryme.top/gtgqebbpwy.html

now=$(date +%F); echo "$now"
来源：http://hz.birdmap.top/gtycvdgrhm.html

[R27] 算术展开
来源：http://hz.birdmap.top/gtsynyvxze.html

echo $((1 + 2 * 3))
来源：http://hz.nwbrower.top/gtywohclyk.html

[R28] 浮点运算
来源：http://hz.cqqwz.cn/gtlmoiyjnf.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhongyouzk.top/gtuiortgtn.html

[R29] 定义函数
来源：http://hz.svipenyu.cn/gtbamyzmwz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.0kj1m.cn/gtacinlzlu.html

[R30] 函数返回状态码
来源：http://hz.jlsjyb.cn/gtdyewwfgi.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgfzy.top/gtjqxjxyli.html

[R31] 局部变量
来源：http://hz.iojbl.cn/gtjrqjjody.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj20258888.top/gtplmdhlfl.html

[R32] 参数个数校验
来源：http://hz.chenzaomai.com/gtqjwmmeyt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.snrcjt.cn/gtdfwcpayc.html

[R33] 捕获错误并提示行号
来源：http://hz.52xcode.cn/gtfkijcpsu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.hongshengwenyu.top/gtcjmxnklp.html

[R34] 退出时清理
来源：http://hz.ppjwa.cn/gtzharlriw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gtsfhwbehc.html

[R35] 后台执行并等待
来源：http://hz.shangyingyoupin.top/gtnnoreqgp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhoulong.xyz/gtiwdebnvc.html

[R36] 并发执行多个任务
来源：http://hz.9152youxi.cn/gtplikmbih.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shuidangran.top/gtlzmbrmcg.html

[R37] 把输出赋给变量
来源：http://hz.zycfv.cn/gtxokdncsp.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtmmyrspcy.html

[R38] 管道串联
来源：http://hz.cheryme.top/gtupmdqckm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.chenjidiqi.icu/gttdbkzoom.html

[R39] 重定向标准输出与错误
来源：http://hz.sweek.top/gtjcfjmvqf.html

cmd > out.log 2>&1
来源：http://hz.wangshuangyany.cn/gttmovqpxm.html

[R40] 追加写日志
来源：http://hz.dianchejie.cn/gtsyiuozey.html

echo "log" >> out.log
来源：http://hz.hysaishi.cn/gtdnszmjle.html

[R41] 丢弃输出
来源：http://hz.guowangkeji.top/gtpxovelaw.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gtldmozpcm.html

[R42] 输入重定向
来源：http://hz.zhoulong.xyz/gtphfyzmyr.html

wc -l < a.txt
来源：http://hz.nanxuanxn.top/gtlbrukqwk.html

[R43] 按名字查找文件
来源：http://hz.wangdashe.top/gthuvrgnqo.html

find . -name "*.log" -type f
来源：http://hz.hnqzz.top/gtiflasglc.html

[R44] 按修改时间查找
来源：http://hz.ehwqpu.com/gttvbdmmbp.html

find . -mtime -7 -type f
来源：http://hz.daria6918.cn/gtutllxyby.html

[R45] 批量删除
来源：http://hz.wangdashe.top/gthgrtibku.html

find . -name "*.tmp" -delete
来源：http://hz.svipenyu.cn/gtjicqdfpy.html

[R46] 递归替换文件内容
来源：http://hz.sweek.top/gtmguyadqn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ydjk.org.cn/gtzojvpdxt.html

[R47] sed 单行替换
来源：http://hz.yj20258888.top/gtqxhbeagb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zycfv.cn/gtsobclhey.html

[R48] awk 取指定列
来源：http://hz.chenlongwang.top/gtfjtaqtmu.html

awk '{print $1, $3}' a.txt
来源：http://hz.9152youxi.cn/gtaarzwkio.html

[R49] awk 带条件
来源：http://hz.hnqzz.top/gtkugtuszu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gzhubu.top/gtnotxndqg.html

[R50] awk 求和
来源：http://hz.jianghu66.top/gtqiqwtvza.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtnhtraimz.html

[R51] 排序去重取前几
来源：http://hz.yj20258888.top/gtrloemhwh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangtech.top/gtxynzldpy.html

[R52] 统计行数
来源：http://hz.gzhubu.top/gtzwjwfplz.html

wc -l a.txt
来源：http://hz.mhx1999.top/gtosylzpcb.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtenxgcpog.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxinkj.top/gtvdzgioew.html

[R54] 比较两个文件
来源：http://hz.smart0.xyz/gtqiimgfee.html

diff a.txt b.txt
来源：http://hz.yj202588.top/gtkxjvhozu.html

[R55] 压缩与解压
来源：http://hz.yvedp.cn/gtzqftuhqf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gzhubu.top/gtgvsoxaws.html

[R56] 远程拷贝
来源：http://hz.ywan-chungtsiang.top/gtzbqxdfaz.html

scp file user@host:/path/
来源：http://hz.haohaochexian.top/gtdrtvsggv.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtyovwdcxb.html

ssh user@host 'uptime'
来源：http://hz.feifeiyinyue.top/gtdrisihiz.html

[R58] 下载文件
来源：http://hz.hfpthk.cn/gtrluljvcg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cdnleiting.top/gttuylulxs.html

[R59] 发 POST JSON
来源：http://hz.ydzc1.top/gteimfnmto.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.smart0.xyz/gtzcqgmgll.html

[R60] 只看 HTTP 状态码
来源：http://hz.shzxlz.cn/gteplcppzd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cqqwz.cn/gtrzzpyrnv.html

[R61] 磁盘占用
来源：http://hz.hnqzz.top/gtrgcinmjy.html

df -h;  du -sh *
来源：http://hz.xylfe.cn/gtlrfkucnu.html

[R62] 找最占空间的文件
来源：http://hz.meibo888.top/gtnujzdkfs.html

du -ah . | sort -rh | head -10
来源：http://hz.birdmap.top/gtnuknypte.html

[R63] 内存与进程
来源：http://hz.tanke756.top/gturrlqakf.html

free -h;  ps aux | grep nginx
来源：http://hz.feifeiyinyue.top/gtvslzmtlg.html

[R64] 结束进程
来源：http://hz.pycfn.com/gtucxvctzk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gttperytzh.html

[R65] 查看端口占用
来源：http://hz.hysaishi.cn/gtrcwoymfm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgufenzy.top/gtzyskahia.html

[R66] 定时任务
来源：http://hz.andypj.xyz/gtibcibxle.html

crontab -e;  crontab -l
来源：http://hz.vqdsnc.cn/gtspwoanaj.html

[R67] 生成随机十六进制串
来源：http://hz.yongpay.top/gtmvxufdry.html

openssl rand -hex 16
来源：http://hz.vqdsnc.cn/gtlmhuitym.html

[R68] 计算文件校验值
来源：http://hz.cashguo.top/gtakoafzjd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtpzbkyfkp.html

[R69] 生成随机密码
来源：http://hz.shuidangran.top/gteljfepfk.html

head -c 16 /dev/urandom | base64
来源：http://hz.daria6918.cn/gtyiaoomdn.html

[R70] 时间戳与互转
来源：http://hz.birdmap.top/gtmpenfmtq.html

date +%s;  date -d @1700000000
来源：http://hz.chenjidiqi.icu/gtbraadhqr.html

[R71] 日期格式化
来源：http://hz.hywenlv.cn/gtrqgnvlgj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gotoacloud.top/gttyuejppp.html

[R72] 等待端口就绪
来源：http://hz.ydzc1.top/gtikgyievt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.iojbl.cn/gtcijxlqwq.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gtmafsevzy.html

split -l 1000 big.log part_
来源：http://hz.9152youxi.cn/gtsrgbwuhv.html

[R74] 批量重命名
来源：http://hz.wangshuangyany.cn/gthbvpzpqb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj20258888.top/gtcehxajmd.html

[R75] 导出环境变量
来源：http://hz.sufxvd.cn/gtfsjnbnon.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yueranfly.top/gtrkakdquu.html

[R76] 使用临时文件
来源：http://hz.ivvv.top/gtvtwordek.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtgxuxtsxu.html

[R77] 读取用户输入
来源：http://hz.0kj1m.cn/gtilyddtcs.html

read -rp "请输入: " ans
来源：http://hz.gzhubu.top/gtvuzyooja.html

[R78] 交互式菜单
来源：http://hz.jinqigfzy.top/gtsfpezxru.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cucudq.cn/gtqjtvhihj.html

[R79] 解析命令行选项
来源：http://hz.jinqigfzy.top/gtxllazcdk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.c1oappe.top/gtadpozsli.html

[R80] 查看脚本执行耗时
来源：http://hz.sweek.top/gtaikzkneo.html

time ./run.sh
来源：http://hz.wangshuangyany.cn/gthdshvwra.html

================================================================================
来源：http://hz.tanke756.top/gtvpshdohw.html

S. C / C++ 专题
来源：http://hz.hywenlv.cn/gtcngwycez.html

================================================================================
来源：http://hz.sxryk.cn/gtquvwbhtx.html

[S01] C：Hello World
来源：http://hz.316326.xyz/gtdupcscvw.html

#include <stdio.h>
来源：http://hz.fzhhl.top/gtknudrsyq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cdnleiting.top/gtshmcpvkk.html

[S02] C：变量与格式化输出
来源：http://hz.jlsjyb.cn/gtfqvhhpch.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuanzx.com/gtkytvnuuj.html

[S03] C：读入整数
来源：http://hz.shangyingyoupin.top/gtqtcfjngq.html

int x; scanf("%d", &x);
来源：http://hz.jinghuilouyu.cn/gtjvxkmcra.html

[S04] C：字符串复制
来源：http://hz.gotoacloud.top/gthktecktg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhiwuduotai.top/gtmzveoqug.html

[S05] C：字符串长度
来源：http://hz.yj20258.top/gtctuqsahf.html

strlen(s)
来源：http://hz.zhoulong.xyz/gtxelrycwh.html

[S06] C：字符串比较
来源：http://hz.ivvv.top/gtncqxjgbz.html

strcmp(a, b) == 0
来源：http://hz.9152youxi.cn/gtduqubuqc.html

[S07] C：数组遍历求和
来源：http://hz.chenjidiqi.icu/gtpjzouvqs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.mhx1999.top/gtbydjfssm.html

[S08] C：动态内存分配与释放
来源：http://hz.aibaodan.cn/gtwbpazlln.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.mhx1999.top/gtxgzfzwon.html

[S09] C：结构体定义与初始化
来源：http://hz.316326.xyz/gtqnmeccwz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sweek.top/gthxvyfkpy.html

[S10] C：指针与解引用
来源：http://hz.yuxming.cn/gtcxjlilzt.html

int *p = &a;  *p = 5;
来源：http://hz.zycfv.cn/gtaegcihrl.html

[S11] C：逐行读文件
来源：http://hz.aibaodan.cn/gtjgugbfep.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jiagoushi.top/gtppbugbxq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fengsongda.top/gtntokfokt.html

fclose(f);
来源：http://hz.cqqwz.cn/gtcsxuwxbs.html

[S12] C：写文件
来源：http://hz.jyoumei.cn/gtsvtcndrg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuxming.cn/gtgkaovbff.html

[S13] C：宏定义
来源：http://hz.nanxinkj.top/gtezfsbmcg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.feifeiyinyue.top/gtmzsvhjva.html

[S14] C：枚举
来源：http://hz.haohaochexian.top/gtcvcoeemm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yj202588.top/gtwzhsztkw.html

[S15] C：类型转换
来源：http://hz.ehwqpu.com/gtqzqxrfgo.html

(double) a / b
来源：http://hz.zhoulong.xyz/gtgqmtjnbv.html

[S16] C：位操作置位
来源：http://hz.bjfxy.top/gtnrjdsbxi.html

x |= (1 << 3);
来源：http://hz.ehwqpu.com/gtcsztqxbf.html

[S17] C：安全拼接字符串
来源：http://hz.jlsjyb.cn/gttljaldky.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gthsrkuvuk.html

[S18] C：命令行参数
来源：http://hz.yueranfly.top/gtdsfozptp.html

int main(int argc, char **argv)
来源：http://hz.jianghu66.top/gtynwxdwux.html

[S19] C：快速排序
来源：http://hz.smart0.xyz/gtprogsgab.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtwtavcpgz.html

[S20] C：二分查找
来源：http://hz.xziqi.cn/gticycmisj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aizwys.cn/gtkvhesges.html

[S21] C：字符类别判断
来源：http://hz.fengsongda.top/gtgnbqzofk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xingfuxueyuan.xyz/gtucbkfmeh.html

[S22] C：字符串转数字
来源：http://hz.gotoacloud.top/gtwxturexy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ehwqpu.com/gtsezvgeuy.html

[S23] C：随机数
来源：http://hz.jinghuilouyu.cn/gttsanpplz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yongpay.top/gtbbftepua.html

[S24] C：获取本地时间
来源：http://hz.dashuyun.cn/gtkazpubex.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydjk.org.cn/gtwizgtsmp.html

[S25] C：内存拷贝
来源：http://hz.guowangkeji.top/gtsxnaikqc.html

memcpy(dst, src, n);
来源：http://hz.dashuyun.cn/gtaywztaei.html

[S26] C：内存清零
来源：http://hz.svipenyu.cn/gtqgtwbmbs.html

memset(a, 0, sizeof a);
来源：http://hz.sweek.top/gttabvmrcw.html

[S27] C：定义常量
来源：http://hz.cdnleiting.top/gtqryhtora.html

const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtukfwjguk.html

[S28] C：静态变量
来源：http://hz.kuanghao11.cn/gtkhzlljou.html

static int counter = 0;
来源：http://hz.hywenlv.cn/gtoynmvpur.html

[S29] C：变参函数
来源：http://hz.52xcode.cn/gtnljshhlq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sweek.top/gtsbdtrtmv.html

[S30] C：头文件保护
来源：http://hz.c1oappe.top/gtvdwvxlsl.html

#ifndef X_H
来源：http://hz.ydzc1.top/gtvnbnhqar.html

#define X_H
来源：http://hz.ivvv.top/gtlqjuhole.html

#endif
来源：http://hz.chenlongwang.top/gtvbtuctrg.html

[S31] C++：Hello World
来源：http://hz.zhixingplan.top/gtwfcivtlf.html


<!-- 参考信息 -->