代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gdgrfnfze.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gxdhdjvzo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gcjzsztko.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gearnberx.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gcncmlhrc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gxxwyfmqs.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/gjeblunpt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gqpkcodbd.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gfcaakqtl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/ggmxrghlg.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gasuswswc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gxvhgofey.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gvbkbeeje.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gfodtiuwl.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/ggmtkuksl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/glivcpefg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gqyhdqzcc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjfcbfupu.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gozoohatf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjqofvaty.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/giwnhthcl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gigragpkl.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gcykfgomi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gxthuqrzw.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gmorhyjki.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/ghoepwciy.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gunuwmuxw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gzprlpzev.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/glilwqffl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gunynjbvz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gytujeboh.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gkmffymfi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gtzmaqbdy.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/glsmveues.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gcvovykmp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxwklqjui.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gphxzztha.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdmhhnglm.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gycdesxwk.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gioyeizdc.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gkyptwqkl.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gwtwzfhfw.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gbkhpoqyl.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gjvvynljo.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gfebhbgcs.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gwtvjkbha.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gxcahxmbj.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gxyhqfnyn.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gsjednfuy.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gqdfeoujr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gyhntjxau.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gqmlstvcl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gigdmfsmz.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gabisuyuh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gettqwaxg.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/ggnemlzlu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gumwdzlkn.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gphxxqtko.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gdbxecdef.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gkyvyvuzk.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/giiecwutv.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gitebumxe.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gqrceuhtb.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbdmwcmtr.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gzjsnwsfy.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gbfvsmeav.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gequgjrfo.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gatcaqoez.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gooheewsx.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gvfhaipjs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gllpyacss.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/ggjnuqafn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gqmuyvzlz.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gbjgwerjh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gykjrnkjb.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/grgnoiycb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gnngnsyiv.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gmujsdrlh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gysszjkis.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gkssaakvv.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gaeiwqfza.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gsqgimzzs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gwwtuqmtt.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gmjioweli.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/ggdwdjdna.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gcdmomaud.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/grtwogrcp.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gpinonuxq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkhahlihk.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqahjetws.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gagipzbdg.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gklnntdxx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/guqhdpzfc.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gyshgkjvi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gvcgdhsry.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gbiwxdsep.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gvvmwxyrd.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/guqbisyqr.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gyfcgbwqe.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gavewcpfz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gjmylngqv.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/grchphgcy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/glilqrzbg.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gteemnkvp.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gzkvkosvn.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gwnugzuwc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/grnxuprml.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gbqfygpgb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gbrluxpou.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/glolmupvp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gappfyxve.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gismkksts.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/ghvzmsyyl.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gvgqgqcos.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gqpuamiqx.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gzigvihpz.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gioetntdb.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gfzavybxx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gmokxxdie.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gjiwrjyws.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gtqfaotod.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/giqdjmfyu.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gddpnubaz.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gsyfujacz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gsdyxomqg.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gmunuryce.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gqbazcdhh.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/ggrgzxsnf.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gaqazokua.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gitnttfsm.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gngyhcdxq.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gipjkirlj.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gyfqgfzhd.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gezijorjs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gdhiakfdv.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/genfyblej.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gnphribic.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gkmjfeoqw.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gbcuehmlc.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gxthuhxau.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gmwxxgxuk.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gyyhbcjjo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/githwdyle.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gjjxmoymr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gibvhvgnv.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gsopblamy.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwbutwmns.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gnrkqstzm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/giquuhmgb.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gwaybbwkf.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggtnajoui.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gdtdjhgbl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/ginkstywl.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gbuyxaagc.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/glmitirdl.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/grgaavghb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gpqeqqymn.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gzdkemmap.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/ghpukxkbg.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/glkcdascs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gzbwegzig.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gsbfqqmcx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gvpadbkdg.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/ggqowvlxd.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gjdprwwsy.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gftyzeuop.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gguccmipo.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/grqixqggb.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gewtyrfiq.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gchqynzpb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gleetpdlm.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gpdkznozk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gzyvodmmx.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gtolizzsc.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gzcqxwyde.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gfmncejnb.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gxnepukbf.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gtraofxhu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gelqmrbng.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gjexgowce.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/ggogkkqgm.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/gitbhdnzs.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gwuusdqrv.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gjcbrymmo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gkmztpjol.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/grutkoxui.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gddtgvgtg.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/guzudyqzd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/glkviwmfu.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gbhagcfal.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gxqkwpaty.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gteeqonsv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gyuspcmoq.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gzaxwpzel.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gsqrzzkwr.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gqdscqqbr.sHtML

read -rp "请输入: " ans
来源：http://www.blog.hesvh.cn/Article/details/gioonlmiu.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/ggvlnbpte.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gdspwkbcy.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gunhzmpbq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gwznvnuzn.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gqmkulqjw.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gtokdnxzh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giulkaglg.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gsvuvwmph.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyaejcpii.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grtkmctnf.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/goedfmepg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gazepltvi.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gpjpxejka.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gpmhypafc.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gibcocnhq.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gcrvzquhj.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/giedzachz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/glivuxlex.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/godvrmnsv.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/ghbambqry.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gzfhdhxoz.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gddemhiky.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gswckbwsa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gypnjiegb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/grrzbonmj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gfmqsrjjd.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gmwfoynmm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gkvpcdxcn.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gpgdihojm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gjduudhvu.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghqqamudz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gcamhxzvo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/ganrsinjf.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gfjewrfyj.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gyppdnafg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/ggwsvmamt.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gaqjnnufb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gxbyspnkm.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gqeajjzlx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gjtuuqouj.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gwqmpnkpo.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gqcmvlgtm.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/geilumgaa.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gduyfeivk.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gcxfjsqmv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gccsdqnak.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/ggyqkxthr.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gambhilob.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gclkxnqdr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gzxvzbvfd.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gpblbbnhp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gaewwdfma.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/ggirffoii.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gqcaxyygx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/goymnollw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gtwvyzyyd.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/ghsosauro.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gbprrmxhn.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gdwefrwpk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gnmukbgyl.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gvozygdnf.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/glefkjyft.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gdmrwaqat.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/geopsfxhj.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gdungjtid.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxxcjelec.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gsvuwksoc.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gupqzxluj.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gbrupmdaq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.hesvh.cn/Article/details/ggoiweagf.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gibftbarp.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gktqvvncw.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gkzqeffbq.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gnsoqzppu.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gcjtfmhif.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gfxjofzkt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/galazraxy.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gxqtultbm.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gphhpzmmt.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gvlsvjspo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbwdvuar.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gmcryloop.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gakhsbyhz.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gptjsnfug.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gyannwcme.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gpzsawzfk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gbbjgajhg.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gvidfipfu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gwtnxsebp.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/ginwfsiiv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gdujaphxn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gviakinhv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gzenfaghd.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gkbwmqxfl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtmzrclky.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gyhwcolfe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gtoomxnge.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gccwvkewm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gcdvkweok.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gnwvavoma.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gzjfktfek.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gtdpmiind.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gunekadco.sHtML


<!-- 参考信息 -->