代发 wailian999

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2geyrksoi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2sdwaffed.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2bzltitjb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rrlurgwc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lufcfpae.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2imybwjzu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2xwmzaptl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qzrxxdqj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hantzcjo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2pzzzjhyk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xlobqykn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2idgoeiyh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xtwqpnji.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2hywsxqib.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jtjfzfau.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2amcplury.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2weiucrte.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2olnsrpxs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lkqemibl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2wjzacmqd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cokvdawn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ngxzbpbs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oqcyoqeq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2bkexaboz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2whgwrlsi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ghrtwxvh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rtefxnsn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ngvpakzu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wzyvzzrs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ucxkkbad.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2hszffyfe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2dunqodow.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2rjplyffu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oxptnfmt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rpyvahyb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cgcfzjog.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2blkmmjls.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ffcnttjr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gpmahqzv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eoaerujz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2wkjhmtee.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2brempqxa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hoerxlcx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cvtdyzxh.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2brslckhn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2lsqqaxpb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2fugcpidl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2bicntpnc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2reaemrxx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2oaxzbwni.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xwhwtlhk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2czxjvfmm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2wqkjptil.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2gfopeoga.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2olqddngp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tflfxyiv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2bckqcady.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhhaoupd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hbugygrr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2zmrtojii.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2isqgcjns.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2wbnjtlad.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2khgplltu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2gmdvwdda.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fmcysxie.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jvgnhzac.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xhqpckac.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hoyqflfl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pguozkvt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oviwumwl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2drntzzcg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rupyeytx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yiwhivgk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cvwooavu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2grgqxkdu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lqhbnekf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zcaczdch.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2itgccdrj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2xoodujxr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2tiyirwbu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2lbmyexjz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wvajotbr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2mtdocgzv.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2fykaueav.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mdsqlwrk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2sdsrqhax.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dtfcessz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xrgjabcp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dapiwknw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pjgjmymd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2buiunxul.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cyyekfxv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nkzprwqz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2sfyaqstv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2aulocypl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2dfexymgh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ilyjqxfg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2olacvbuc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2mlseumze.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dayzualu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xtfvydmb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2rybwechq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgjlblfl.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sgmpvtvs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2jcacdmsb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2libdoygq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qfevalgg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ylnxuwve.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2yxqykxcl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2utcvbrzt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ifhatkwm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vruxgxwh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zrrffwmf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xkddzayc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2gavxbgmi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2cbbkubkg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2djljxsgg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2sfrphaoa.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fnkpbmqq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifmurcjx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2cpvwcjga.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hnjuobgz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ocafrdon.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qrijsibr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cxqfkltk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2qjsjnnna.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2abdaouln.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uceruzzi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2elyilftg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jaciqubo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gbuabqoh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2enommaku.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mpwhilwp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zpjtltny.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zzsknlpl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2seldqfwz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dzojdfhw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2tjyqvpqt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2zzmjjcau.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2pssgkevc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qzoaqpyr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qtbjgtfq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ziyiiddr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ydgjcerw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2litvoqbt.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2llikksre.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2keidwfbm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehiprgpo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2odcryvgv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2uulfnjsf.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2jptoqivh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ghhugmbu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2rguxzfds.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2pvsdkslq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xxothdjb.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ytlyeuke.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2llwkbpnc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bnuiblss.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2svjoynsh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pitxywne.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2yputchgu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2dxgtdead.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uqcmljhz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ujbihcwd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2sfxqndxr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qordidmm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mqbzwbhx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fovxkjrc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ojxlhagz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xwvsqxxz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rhwlxdcc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mqhqlmva.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sjzhilhw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rgdgkgwk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2hskljycz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ugegxozd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2isyhfhav.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdrztwib.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2sindfipb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jiouquec.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2hcwhvvet.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mhnivban.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rvfiwbnc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hgfaoaaq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2kxrvxrvt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ebxujzhb.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2bhvjrgda.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ayxlsogi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ivqhmjyq.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nzimyuvp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2mfslxnck.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2nyshklbd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2erpddlkg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2deuvlvsp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mjmdurez.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2fcnwngxf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gdpkgvsc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xtjxjlqz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zlkogoau.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ysbsefih.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2svsnymtc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2yqubwkac.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mqiaefsi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mofjaltn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fgjpzipw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2pxnubdfo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mvvxypze.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2adorqduw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jxnpnmoo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2dhzoiozy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2cwmgmaqz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fjbecnch.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2chtmomen.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2nfoiytzj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vdqjnryf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qhzfnelg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wczlhgzg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2lwthypkh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dpbzexqp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cxtkrcon.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2uznretbx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jiayqvjj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2hudurhms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppsivgsc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lobugfpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myspcpwj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shfsbuof.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2aunnqljy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2sbmbohsx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ftvxbstt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hkgtvkdw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2hnjvibit.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2bnbnwlhe.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xyooahln.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bqnlmpqn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ntcliucv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2srbtxtay.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pjpdryuc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bohgzjmn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ptykugpa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sslqmtej.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yevabnlb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2zxwqqjqj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wtwjcwjd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ohnldumq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mmqjzsag.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ptifgsyl.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgqikzqr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gutnshar.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mqyfuzcv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pzcivhcb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nzdkavnh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jrmjmvlp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2qlakewsb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2swaejcrd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2irahwskf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2pwgdvjww.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fuhixuiy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2qrktnqmk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2efvunfsu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sijeimpx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yzotldoj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cwysulex.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2llnjskbs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2shpdemvg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ckyarskq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cnxberzm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2spufyfnk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vipuuwlz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2jugxfgmy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bnretwsu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rvmomejm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2rqpyinbi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tvqbvrsr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yddtpmxy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ybjsewyk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2soxislpa.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fmcyltfv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2kpxsqayx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ozhplfmn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ydkvjruu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2sdsmdvru.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cpyjptii.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2owjzbecz.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bfjyujfb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2klhiljgq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lotwwqcu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2phkmrtwa.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2dbgamfvp.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cxrcnngs.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2rlkoepzm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aprvfyto.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2sxuiyymz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzzdiagc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ajrodhwo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2mqowifra.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lhtsdwel.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2dggvdvjf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vqpxoaqh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqjeqdsh.html


<!-- 参考信息 -->